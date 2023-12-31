---
title: "Saccharomyces cerevisiae"
aliases:
  - baker's yeast
  - S. cerevisiae
  - Saccharomyces cerevisiae
tags: 
date: 2023-08-09
---

*Saccharomyces cerevisiae* (baker's yeast) is a well-characterized organism in biology. I've started working them in the summer of 2023, and I find them very friendly (especially compared to the fussiness of metazoan tissue culture).

[[notes/2c_yeast-are-model-organisms|yeast are model organisms for biology]] and boast many [[notes/2d_synthetic-biology|synthetic biology tools]] that make them ideal platforms for high-throughput experimentation.
- To quickly test many combinations of two proteins, one can transform one of the two mating types with each, crossbreed the results, and run an auxotrophic selection to get diploid cells with both proteins.
	- This method scales quadratically: 5x5 means 10 transformations for 25 combinations; 10x10 means 20 transformations for 100 combinations.
- Expression of proteins in yeast can be tweaked by changing the type of [[notes/2c3_yeast-vectors|vector]] used in transformation.
- The [[notes/2c1_yeast-toolkit|MoClo yeast toolkit]] uses a robust [[Golden Gate Cloning]] syntax to quickly build custom constructs from a library of parts.

Yeast have three primary types of [[notes/2c3_yeast-vectors|expression vectors]]: integrating plasmids, cen-ARS plasmids, and 2-micron plasmids. Genes of interest must be cloned into these for yeast experimentation.

Genes can be expressed in yeast using a simple transformation, unlike metazoan cells (which require a more complex transfection or transduction).