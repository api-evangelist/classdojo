---
title: "Large Analytics SQL Queries are a Code Smell"
url: "https://engineering.classdojo.com/2022/08/03/large-analytics-sql-queries-are-a-code-smell"
date: "2022-08-03"
author: "Will Keleher"
feed_url: "https://engineering.classdojo.com/rss.xml"
---
A single large query in SQL can be hard to understand, test, debug, or change in the same way that an over-large function in code can be. A large query is also much harder to write! Feedback loops while writing large queries are slow and you'll often find yourself needing to guess at where the problem in your query is.
