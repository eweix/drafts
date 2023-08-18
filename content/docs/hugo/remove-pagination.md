---
title: "Replacement for hugo pagination"
aliases:
- replacement for hugo pagination
- remove pagination in hugo
- remove pagination
tags:
- snippet
date: 2023-08-14
---
For replacing pagination in [[docs/hugo/hugo|hugo]]. See also [[docs/hugo/page-list|page-list]] snippet for hugo.
a
## Sections
Replace instances of:

```go
{{ range .Paginator.Pages }}
```

With:

```go
{{ $section := .Section }}
{{ range where .Pages "Section" $section }}
```

Source: [https://discourse.gohugo.io/t/turn-off-pagination/9961/8](https://discourse.gohugo.io/t/turn-off-pagination/9961/8)