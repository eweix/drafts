---
title: Custom page lists in hugo
aliases:
- custom page lists in hugo
tags:
- snippet
date: 2023-08-16
---

[https://digitalnotions.net/divide-post-list-by-year-in-hugo/](https://digitalnotions.net/divide-post-list-by-year-in-hugo/)

```HTML
{{ range (where .Site.RegularPages "Type" "in" (slice "POSTS")).GroupByDate "2006-01" }}
<h2>{{ .Key.Format "January 2006" }}</h2>
<ul>
  {{ range .Pages }}
  <li>
    <span class="date">{{ .Date.Format (.Site.Params.dateFormat | default "January 2, 2006" ) }}</span>
    <a class="title" href="{{ .Params.externalLink | default .RelPermalink }}">{{ .Title }}</a>
  </li>
  {{- end -}}
</ul>
{{ end }}
```

Replace "POSTS" with whatever category, collection, or section you're trying to sort. 