---
name: Diagnose YugabyteDB query performance
description: >-
  Use the yugabyted UI API to investigate slow and live queries, correlate with
  cluster metrics and node activity, and identify hot tables.
api: openapi/yugabyte-yugabyted-openapi-original.yaml
operations:
- getLiveQueries
- getSlowQueries
- getClusterMetric
- getClusterActivities
- getClusterTables
---

# Diagnose YugabyteDB query performance

Authenticate with `Authorization: Bearer <api-key>`. Responses are JSON; handle
`400`/`500` ApiError bodies and retry `500`s with backoff.

## Steps

1. Call `getSlowQueries` to pull the aggregated slow-query statistics (YSQL/YCQL).
2. Call `getLiveQueries` to see what is executing right now.
3. Call `getClusterMetric` for the relevant metric window (CPU, IOPS, latency) to
   correlate the slow queries with resource pressure.
4. Call `getClusterActivities` to check for concurrent operations (backups,
   rebalancing) that could be competing for resources.
5. Call `getClusterTables` to identify the tables the slow queries hit and check
   for hotspots.

## Rules

- Read-only flow; never issue schema or data changes from this skill.
- Aggregate slow-query rows by normalized statement before ranking; a single hot
  statement usually dominates.
- Cross-reference conventions/yugabyte-conventions.yml for the auth and error model.
