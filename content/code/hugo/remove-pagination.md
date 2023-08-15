---
title: "Replacement for hugo pagination"
aliases:
tags:
- snippet
date: 2023-08-14
---
For replacing pagination in [[code/hugo|hugo]]. See also [[code/hugo/page-list|page-list]] snippet for hugo.

Replace instances of:

```go
{{ range .Paginator.Pages }}
```

With:

```go
{{ $section := .Section }}
{{ range where .Pages "Section" $section }}
```

This also works with terms and whatnot. Simply replace section with term, and you should be good to go.

Source: [https://discourse.gohugo.io/t/turn-off-pagination/9961/8](https://discourse.gohugo.io/t/turn-off-pagination/9961/8)