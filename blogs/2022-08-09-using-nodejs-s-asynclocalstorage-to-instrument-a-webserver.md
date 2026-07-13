---
title: "Using NodeJS's AsyncLocalStorage to Instrument a Webserver"
url: "https://engineering.classdojo.com/2022/08/09/async-local-storage-in-detail"
date: "2022-08-09"
author: "Will Keleher"
feed_url: "https://engineering.classdojo.com/rss.xml"
---
In the dark times before [`AsyncLocalStorage`](https://nodejs.org/api/async_context.html#class-asynclocalstorage), it could be hard to tell why a request would occasionally time out. Were there multiple relatively slow queries somewhere in that route's code? Was another request on the same container saturating a database connection pool? Did another request block the event loop? It was possible to
