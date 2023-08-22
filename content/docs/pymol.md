---
title: "PyMol"
aliases:
  - PyMol
tags:
  - stack
date: 2023-08-15
---

## Useful Commands
### Selection and Highlighting
To select a specific peptide sequence, use the following command:

```
select pepseq <sequence>
```

Use only single-letter amino acid abbreviations. This can easily be copied over from benchling or some other program and works very well with structural predictions from [[docs/alphafold|AlphaFold]].

### Coloring sequences
After [[docs/pymol#Selection and Highlighting|selecting a peptide sequence]], it's often useful to color that. When I play around with proteins where the domains are known, the first thing I do is color those domains so I can easily see them on the structure. Just right-click on the selected sequence and select `color` from the menu. Some sort of consistent scheme can be useful for this.