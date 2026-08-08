---
title: "Two tablets stuck in Creation mode"
url: "https://forum.yugabyte.com/t/two-tablets-stuck-in-creation-mode/5133#post_3"
date: "2026-08-04"
author: "@maxernstscr"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
{"underreplicated_tablets":[{"table_uuid":"00004001000030008000000000004193","tablet_uuid":"1a092f17af2c4c98bef2e8aa35578273","underreplicated_placements":["78084298-4b65-48f0-9082-93f88ec4846f"]},{"table_uuid":"00004001000030008000000000004193","tablet_uuid":"d51000ef61e04a48b8614389526a2777","underreplicated_placements":["78084298-4b65-48f0-9082-93f88ec4846f"]}]} {rosh-1.7.3}yugabytedb_prod@$hostname:/local/data/scratch/yugabyte/data/yb-data/master/logs$ grep -n ‘1a092f17af2c4c98bef2e8aa35578273|d51000ef61e04a48b8614389526a2777’ yb-master. .INFO. yb-master.
