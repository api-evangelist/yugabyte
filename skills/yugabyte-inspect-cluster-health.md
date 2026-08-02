---
name: Inspect YugabyteDB cluster health
description: >-
  Use the yugabyted UI API to assess a YugabyteDB cluster's health - status,
  nodes, health check, active alerts, and load-balancer state - before or during
  an incident.
api: openapi/yugabyte-yugabyted-openapi-original.yaml
operations:
- getCluster
- getClusterNodes
- getClusterHealthCheck
- getClusterAlerts
- getIsLoadBalancerIdle
---

# Inspect YugabyteDB cluster health

Authenticate with `Authorization: Bearer <api-key>` (BearerAuthToken scheme). All
responses are JSON; every operation can return `400` (bad request) or `500`
(ApiError) - surface the ApiError body on failure and retry `500`s with backoff.

## Steps

1. Call `getCluster` to read cluster metadata and overall status.
2. Call `getClusterNodes` to enumerate nodes and confirm each is up.
3. Call `getClusterHealthCheck` to run the health check and read any warnings.
4. Call `getClusterAlerts` to list active alerts.
5. Call `getIsLoadBalancerIdle` to confirm the load balancer has settled (not
   idle == rebalancing in progress).

## Rules

- Read-only flow - none of these operations mutate state (see
  agentic-access/yugabyte-agentic-access.yml: all classified `connected`/`read`).
- If the health check reports under-replicated tablets or dead nodes, do not act
  automatically; escalate to a human operator.
