---
hide_hero: true
# callouts: callouts
---

## Pages

A page is a fixed page that contains static information. Pages are used for generic information. The server also as landing pages. 

## Blog Posts

The web-site has two main content types: 

- Pages
- Blog entries

New videos should be included as blog entries.

All blog entries must be filed under _posts and have the following filename: `YYYY-MM-DD-author.md`. If you have more than one blog post per day number the blog post. 

Each blog post should include a preamble: 

```
---
layout: post
title:  Title of the blog
categories: 
- development
- test
---
```

Posts without this preamble will receive a notification. 

Categories MUST be a YAML list.

## Projects

`dxiai`-projects pages reside under the main page if github pages are active. These locations MUST NOT be used. 

[<i class="fas fa-home"/> &nbsp; Back to Home](https://www.dxi.ai/tmppages/){: .btn.btn-success}
