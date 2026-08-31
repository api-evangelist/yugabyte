---
title: "Tcmalloc issues"
url: "https://forum.yugabyte.com/t/tcmalloc-issues/5141#post_3"
date: "2026-08-26"
author: "@amizne_yugabytedb Amiram Mizne"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
Hi @marknefedov - Thank you for the detailed report. The crashes come from tcmalloc’s per-CPU cache, depending on rseq behavior that kernel 6.19 changed. Upstream treated the change as a kernel regression and reverted it, so the fix is on the kernel side.
