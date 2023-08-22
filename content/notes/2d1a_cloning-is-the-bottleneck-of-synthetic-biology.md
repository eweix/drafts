---
title: "Cloning is the bottleneck of synthetic biology"
aliases:
  - synthetic biology cloning tools
tags: 
date: 2023-08-15
---

[[notes/2d_synthetic-biology|Synthetic biology]] relies largely on [[notes/2d1_cloning|gene cloning]] to test various [[notes/2a3a_operon-model|genetic circuits]] *in vivo*. Depending on cloning strategies, it can take anywhere from several days to several weeks to get from design to data. Since [[notes/5_theory-of-constraints|addressing bottlenecks is the best way to improve efficiency]], there are several strategies to deal with this.

Consider the example cloning workflow:
1. Design a peptide of interest *in silico* and gather source DNA.
2. PCR source DNA to replicate the bits that express target proteins.
3. Take target DNA sequences and put them into an expression vector.
4. Transform expression vector into bacteria. Plate it. Pick a few colonies to make overnight cultures.
5. Culture the cells, lyse them, and purify replicated expression vector.
6. Send expression vector for sequencing. If it matches up with the *in silico* design, then it is ready for cloning. Otherwise, pick new colonies and try again.

After that, you can move on to experimentation. The whole process to go from idea to usable construct can take a week or two, though it varies depending on what libraries you might have available and sequencing luck.

## Tools
- The [[notes/2c1_yeast-toolkit|MoClo yeast kit]] uses [[Golden Gate Cloning]] to improve iteration and combinatorial variation by building out a library of parts that can rapidly be assembled into functional constructs, with practically non-existent error rates.
- Diagnostic digest vs sequencing - sequencing is more accurate, but digests only take ~1 hour to produce results.
- Colony PCR - very fast and cheap for lots of constructs, but requires specific primer placement and planning.