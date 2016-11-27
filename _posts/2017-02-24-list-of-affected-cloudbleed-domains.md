---
layout: post
title: List of affected Cloudbleed domains
---

```c
if ( ++p == pe ) // ☁️ 💔
```

### Sure

{% for domain in site.data.cloudbleed.sure %}
- [{{ domain }}](https://{{ domain }}){% endfor %}

### Maybe

{% for domain in site.data.cloudbleed.maybe %}
- [{{ domain }}](https://{{ domain }}){% endfor %}

### Sources

- [Google and DuckDuckGo searches/cache](https://www.youtube.com/watch?v=oHg5SJYRHA0)
- [Hacker News's comments](https://news.ycombinator.com/item?id=13718752)

### Sources's sources

- [Tavis's report](https://bugs.chromium.org/p/project-zero/issues/detail?id=1139)
- [Cloudflare's write-up](https://blog.cloudflare.com/incident-report-on-memory-leak-caused-by-cloudflare-parser-bug/)

### Sweet karma

- [Twitter's tweet](https://twitter.com/bydorian/status/835055649809539072)
- [Hacker news's item](https://news.ycombinator.com/item?id=13722199)
- [Reddit's post](https://www.reddit.com/r/netsec/comments/5vwjwi/list_of_affected_cloudbleed_domains/)
