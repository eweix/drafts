---
title: Sort pages by date in hugo
aliases:
  - sort pages by date in hugo
  - sort pages by date
  - pagesort date
tags:
  - snippet
date: 2023-08-16
---

A snippet to group things by date in a section. I use this to display things from the reading list, which makes it easy for me to see what I read and when.

[https://digitalnotions.net/divide-post-list-by-year-in-hugo/](https://digitalnotions.net/divide-post-list-by-year-in-hugo/)

```HTML
{{ range (where .Site.RegularPages "Type" "in" (slice "POSTS")).GroupByDate "2006" }}
<h2>{{ .Key }}</h2>
<ul>
  {{ range .Pages }}
  <li>
    <span class="date">{{ .Date.Format "2006-01-02" }}</span>
    <a class="title" href="{{ .Permalink }}">{{ .Title }}</a>
  </li>
  {{- end -}}
</ul>
{{ end }}
```

Replace `POSTS` with whatever category, collection, or section you're trying to sort. 