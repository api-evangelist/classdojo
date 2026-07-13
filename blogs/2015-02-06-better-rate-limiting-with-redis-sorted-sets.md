---
title: "Better Rate Limiting With Redis Sorted Sets"
url: "https://engineering.classdojo.com/2015/02/06/rolling-rate-limiter"
date: "2015-02-06"
author: "Peter Hayes"
feed_url: "https://engineering.classdojo.com/rss.xml"
---
At ClassDojo, we've recently been building out our push notification infrastructure. Our plans required a rate limiter that met the following criteria:
