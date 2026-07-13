---
title: "Canary Containers at ClassDojo in Too Much Detail"
url: "https://engineering.classdojo.com/2021/11/02/canary-containers-in-too-much-detail"
date: "2021-11-02"
author: "Will Keleher"
feed_url: "https://engineering.classdojo.com/rss.xml"
---
[Canary releases](https://martinfowler.com/bliki/CanaryRelease.html) are pretty great! ClassDojo uses them as part of our continuous delivery pipeline: having a subset of real users use & validate our app before continuing with deploys allows us to safely & automatically deploy many times a day.
