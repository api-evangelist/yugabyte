---
title: "Using Yugabytes with Lakefs 1.7x"
url: "https://forum.yugabyte.com/t/using-yugabytes-with-lakefs-1-7x/5004#post_5"
date: "2026-06-03"
author: "@scott"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
The latency impact will largely depend on the network round-trip time between datacentres, since synchronous replication requires acknowledgements from a majority of replicas before a write is considered successful. As the number of datacentres increases, write latency can increase because more geographically distributed nodes participate in the consensus process. This is a common consideration in distributed database architectures and consensus-based systems such as those described in the Raft Consensus Algorithm .
