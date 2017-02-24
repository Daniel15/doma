---
layout: post
title: List of affected Cloudbleed domains
---

Technically [any Cloudflare-controlled domain](https://github.com/pirate/sites-using-cloudflare) could be affected but those are the ones that had public leaked data even after the disclosure:

```c
if ( ++p == pe ) // ☁️ 💔
```

### Found in the wild

{% for domain in site.data.cloudbleed.sure %}
- [{{ domain }}](https://{{ domain }}){% endfor %}

### Found in the wild by other people

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

### Contributing

- [cloudbleed.yml](https://github.com/Dorian/doma/blob/master/_data/cloudbleed.yml)
