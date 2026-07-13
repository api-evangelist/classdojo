---
title: "Graceful web-server shutdowns behind HAProxy"
url: "https://engineering.classdojo.com/2021/07/13/haproxy-graceful-server-shutdowns"
date: "2021-07-13"
author: "Will Keleher"
feed_url: "https://engineering.classdojo.com/rss.xml"
---
Fully graceful incremental deploys are hard. Any number of events can deliver brief spates of 5xx errors to your clients, and getting all of the pieces right isn't trivial. And, if something isn't quite right, it can be hard to detect problems from a few seconds of downtime on a server over the course of a deploy.
