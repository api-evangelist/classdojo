---
title: "Creating an Actionable Logging Taxonomy"
url: "https://engineering.classdojo.com/2021/07/20/actionable-logging-taxonomy"
date: "2021-07-20"
author: "Will Keleher"
feed_url: "https://engineering.classdojo.com/rss.xml"
---
The standard syslog-based way to handle logs is to divide logs into categories like `FATAL`, `ERROR`, `WARN`,`INFO`, and `DEBUG` and use those categories to adjust which logs you see. Having a standard logging taxonomy is incredibly useful when you're dealing with logs for many different systems, but for our backend web-servers, we didn't find these syslog-based divisions to be actionable or easily searchable. We instead created our own categories that map to how we want to handle our logs.
