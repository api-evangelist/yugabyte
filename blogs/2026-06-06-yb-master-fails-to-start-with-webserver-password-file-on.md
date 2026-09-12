---
title: "yb-master fails to start with --webserver_password_file on v2025.2.3.0-b149: Invalid option global_passwords_file"
url: "https://forum.yugabyte.com/t/yb-master-fails-to-start-with-webserver-password-file-on-v2025-2-3-0-b149-invalid-option-global-passwords-file/5012#post_2"
date: "2026-06-06"
author: "@dorian_yugabyte Dorian Hoxha"
feed_url: "https://forum.yugabyte.com/posts.rss"
---
Hi @ivanchevskaya Thank you for the report, I filed this bug report [DocDB] yb-master/yb-tserver fail to start when --webserver_password_file is set (Web UI auth) · Issue #32074 · yugabyte/yugabyte-db · GitHub . ivanchevskaya: Also, is there any currently supported way to enable authentication for yb-master and yb-tserver Web UI ports 7000 and 9000 , or is the recommended approach to protect these ports using an external reverse proxy/auth layer? A reverse proxy is the recommended approach for now.
