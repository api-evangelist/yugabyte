---
title: "Is Yugabyte compatible with Gorse?"
url: "https://forum.yugabyte.com/t/is-yugabyte-compatible-with-gorse/5209#post_2"
date: "2026-09-14"
author: "@dorian_yugabyte Dorian Hoxha"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
Hi @kokoskiwi It should work as a data_store . Make sure to set yb-tserver configuration reference | YugabyteDB Docs to False so it has higher compatibility on table sharding.
