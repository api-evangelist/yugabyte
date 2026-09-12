---
title: "YugabyteDB into Apache Arrow through ADBC, using psqlodbc 16 (PG wire) (adbcBridge 0.1.0)"
url: "https://forum.yugabyte.com/t/yugabytedb-into-apache-arrow-through-adbc-using-psqlodbc-16-pg-wire-adbcbridge-0-1-0/5201#post_2"
date: "2026-09-05"
author: "@singhpratech"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
A follow-up with one new measurement and one correction that matters for YDB users. On 2026-09-05 I ran the same seven-step ADBC workload (connect, SELECT 1, DDL + inserts + read, 1,000-row adbc_ingest , GetTableSchema, GetObjects, read back) through the Apache Arrow native PostgreSQL ADBC driver (1.12.0) and through adbcBridge over psqlodbc, against YDB’s PostgreSQL-wire endpoint. Native driver: connects, then stops at SELECT 1 with could not begin COPY: … RawStmt: alternative is not implemented yet : 138 .
