---
title: "Cloning is the bottleneck of synthetic biology"
aliases:
  - synthetic biology cloning tools
tags: null
date: 2023-08-15
---

[[notes/2d_synthetic-biology|Synthetic biology]] relies largely on gene cloning to test various [[notes/2a3a_operon-model|genetic circuits]] *in vivo*. Depending on cloning strategies, it can take anywhere from several days to several weeks to get from design to data. Since [[notes/5_theory-of-constraints|addressing bottlenecks is the best way to improve efficiency]], there are several strategies to deal with this.

## Tools
- The [[notes/2c1_yeast-toolkit|MoClo yeast kit]] uses [[Golden Gate Cloning]] to improve iteration and combinatorial variation by building out a library of parts that can rapidly be assembled into functional constructs, with practically non-existent error rates.
- Diagnostic digest vs sequencing - sequencing is more accurate, but digests only take ~1 hour to produce results.
- Colony PCR - very fast and cheap for lots of constructs, but requires specific primer placement and planning.