---
title: "HyperLogLog-orrhea"
url: "https://engineering.classdojo.com/2021/07/23/hyperloglog-orrhea"
date: "2021-07-23"
author: "Will Keleher"
feed_url: "https://engineering.classdojo.com/rss.xml"
---
Say you had a few petabytes of user ids lying around somewhere, and someone told you that they were going to use a few kb of memory to estimate the "cardinality", or the number of distinct ids, of those petabytes of ids with decently high accuracy. It'd feel like magic! The HyperLogLog algorithm makes that magic cardinality estimation happen through the Power of Random Numbers, and some clever use of data structures.
