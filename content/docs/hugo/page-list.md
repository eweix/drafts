---
title: "Page lists"
aliases:
  - 
tags: snippet
date: 2023-08-14
---

```HTML
{{ $section := .Section }}
{{ range where .Pages "Section" $section }}
    <ul><a href="{{ .Permalink }}">{{ .Title }}</a> &dot; <i>{{ .Lastmod.format "2015-01-21" }}</i></ul>
{{ end }}
```

This piece of code for [[docs/hugo/hugo|hugo]] produces a list of pages in a section in no particular order, listing their title and last modified date.