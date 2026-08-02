---
title: "Blacklist node in cluster"
url: "https://forum.yugabyte.com/t/blacklist-node-in-cluster/4886#post_4"
date: "2026-02-11"
author: "@dorian_yugabyte Dorian Hoxha"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
The change_blacklist is just for telling yb-masters to not put tablets in yb-tservers. While change_leader_blacklist is to tell not to put tablet-leaders.
