---
title: "Even Better Rate Limiting"
url: "https://engineering.classdojo.com/2021/08/25/even-better-rate-limiting"
date: "2021-08-25"
author: "Andrew Burgess"
feed_url: "https://engineering.classdojo.com/rss.xml"
---
You may have read our post from a few years ago [implementing a rolling-window rate limiter](https://engineering.classdojo.com/2015/02/06/rolling-rate-limiter), where we talked about the implementation of our sliding log rate limiter. That approach has been working well since then, but with increases in traffic, we recently found ourselves rebuilding the rate limiter to improve performance. With some relatively small changes, we were able to improve our redis CPU usage by 40x!
