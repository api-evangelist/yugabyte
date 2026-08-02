---
title: "Wal archive-command like functionality?"
url: "https://forum.yugabyte.com/t/wal-archive-command-like-functionality/5069#post_4"
date: "2026-06-30"
author: "@Alan_Caldera Alan Caldera"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
Hi @hispebarzu - We aren’t planning to implement log shipping because our logs aren’t used for recovery in the way that other relational databases use them. That’s why we implemented Incremental Backups that actually capture changed files and can run on a shorter schedule. The time required for an incremental backup depends on the number of objects in your databases as we must extract the schema at every iteration.
