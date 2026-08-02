---
title: "Yb master cluster balancer"
url: "https://forum.yugabyte.com/t/yb-master-cluster-balancer/4947#post_4"
date: "2026-04-13"
author: "@Anubhav_Srivastava Anubhav Srivastava"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
Increasing the leader_balance_threshold flag might help here, but it wouldn’t fix the underlying cause of the election storm. If you can figure out what is causing that (e.g., a certain query causing high load on a tserver, an internal deadlock, etc.) that would be useful. If you’re looking for more of a patch fix, a more typical approach is to lower the value of load_balancer_max_concurrent_moves to something like 5, so that the cluster balance makes fewer concurrent leader moves in each iteration (the cluster balancer runs around once a second, so that is ~5 leader moves / s).
