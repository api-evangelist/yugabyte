---
title: "Does increasing the number of database users/roles impact performance?"
url: "https://forum.yugabyte.com/t/does-increasing-the-number-of-database-users-roles-impact-performance/5220#post_2"
date: "2026-09-24"
author: "@dorian_yugabyte Dorian Hoxha"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
Hi @kotha.purushotham kotha.purushotham: Does a higher number of users/roles affect query performance or connection handling? Having more roles / users should not have any impact. Though when workload is running , DDL operations involving roles results in catalog version increment for each Database thus causing invalidation message flow to each database.
