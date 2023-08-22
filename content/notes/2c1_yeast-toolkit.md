---
title: "MoClo Yeast Toolkit"
aliases:
  - MoClo yeast toolkit
  - yeast toolkit
  - MoClo kit
  - yeast golden gate kit
tags: 
date: 2023-08-10
---

The Modular Yeast Toolkit[^1] (YTK) is a set of design principles and parts for construct design in yeast (and particularly *[[notes/2c2_saccharomyces-cerevisiae|S. cerevisiae]]*). The YTK uses [[Golden Gate Cloning]] techniques and the MoClo part syntax as a design framework.

## Toolkit Taxonomy
YTK has three "types" of plasmids:
- Part plasmids are not ready for expression in yeast. Instead, these are like your catalog of sequences. These plasmids have BsaI binding sites that are used to define the part type.
- Cassette plasmids are complete transcriptional units. These are assembled from one of each part plasmid. This is the beauty of the YTK—you can easily mix and match and make an entirely new cassete in about half an hour.
- Multigene plasmids are assembled from the transcriptional units in cassette plasmids, and allow expression of multiple genes. This makes transformation much more convenient, since it uses only a single plasmid for expression.

To use a sequence with the toolkit, you have to go through a process of "domesticating" it into the kit taxonomy, assembling it into a part plasmid. From there, you can begin building your transcriptional units.

![[media/moclo-workflow.png]]

## MoClo Golden Gate Syntax
MoClo syntax divides sequences into different types depending on the purpose of the DNA:
1. Assembly connectors. This set goes at the start of the TU. These are used in cassette plasmids to define where that transcriptional unit will fit in a multi-gene plasmid.
2. Promoters.
3. Coding sequences. This is where the sequence for your protein of interest goes.
4. Terminator.
5. Assembly Connectors. These ones go at the end of the TU.
6. Yeast marker.
7. Yeast origin. Where the yeast starts copying the plasmid.
8. Bacterial marker + origin. Where the bacteria start copying the plasmid.

[^1]: Lee, M.E., DeLoache, W.C., Cervantes, B., and Dueber, J.E. (2015). A Highly Characterized Yeast Toolkit for Modular, Multipart Assembly. ACS Synth. Biol. _4_, 975–986. [10.1021/sb500366v](https://doi.org/10.1021/sb500366v).