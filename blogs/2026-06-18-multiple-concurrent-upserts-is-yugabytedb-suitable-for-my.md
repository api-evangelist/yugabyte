---
title: "Multiple concurrent upserts: Is YugabyteDB suitable for my use case?"
url: "https://forum.yugabyte.com/t/multiple-concurrent-upserts-is-yugabytedb-suitable-for-my-use-case/5068#post_4"
date: "2026-06-18"
author: "@dorian_yugabyte Dorian Hoxha"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
ygc: I can partition in Kafka, but then we’ll have “hot device IDs” which get hundreds of reading per minute, while others get close to nothing. This is why we avoid it. Hundreds per minute is, like, 10/second, so this is inline with kafka, and it’s better to handle it here compared to the other level in yugabyte.
