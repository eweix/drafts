---
title: "{{title}}"
aliases:
- "{{title}}"
doi: {{doi}}
authors: {{authors}}{{directors}}
tags:
date: {{date | format("YYYY")}}
abstract >-
	"{{abstractNote}}"
---
## Summary


## Interesting citations


## Notes
{% persist "annotations" %}
{% set newAnnotations = annotations | filterby("date", "dateafter", lastImportDate) %}
{% if newAnnotations.length > 0 %}

<!-- Updated: {{importDate | format("YYYY-MM-DD h:mm a")}} -->

{% for a in newAnnotations %}
> {{a.annotatedText}}
{% endfor %}

{% endif %}
{% endpersist %}