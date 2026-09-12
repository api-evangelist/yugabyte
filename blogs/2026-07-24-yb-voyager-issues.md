---
title: "Yb voyager issues"
url: "https://forum.yugabyte.com/t/yb-voyager-issues/5074#post_4"
date: "2026-07-24"
author: "@dorian_yugabyte Dorian Hoxha"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
dorian_yugabyte: Question: what is the maximum column value for these across all rows? The ENABLE_BLOB_EXPORT directive in the ora2pg conf file can be enabled (i.e., set to 1) to have Voyager export BLOB data from MySQL. The ora2pg conf file should be located here: /etc/yb-voyager/base-ora2pg.conf However, note that there is a there is an RPC message size restriction in YugabyteDB of about ~200 MB.
