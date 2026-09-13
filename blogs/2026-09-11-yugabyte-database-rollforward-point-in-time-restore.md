---
title: "Yugabyte database rollforward Point in time restore"
url: "https://forum.yugabyte.com/t/yugabyte-database-rollforward-point-in-time-restore/5206#post_4"
date: "2026-09-11"
author: "@Alan_Caldera Alan Caldera"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
Sid – Incremental backups copy changed SST files created between backups. See Incremental Backups for a more complete explanation. We don’t need to copy the entire 50TB database; we only need to copy the new files created since the last full or incremental backup.
