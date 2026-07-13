---
title: "Culling Containers with a Leaky Bucket"
url: "https://engineering.classdojo.com/2022/12/05/culling-containers-with-a-leaky-bucket"
date: "2022-12-05"
author: "Will Keleher"
feed_url: "https://engineering.classdojo.com/rss.xml"
---
ClassDojo occasionally has a few containers get into bad states that they're not able to recover from. This normally happens when a connection for a database gets into a bad state -- we've seen this with Redis, MySQL, MongoDB, and RabbitMQ connections. We do our best to fix these problems, but we also want to make it so that our containers have a chance of recovering on their own without manual in
