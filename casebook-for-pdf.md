---
title: Civil Procedure
subtitle: An Open-Source Casebook
author: Eric M. Fink
affiliation: Elon Law School
date: August 2025
repo: CivProCasebook
version: 4.1

epigraph: Jarndyce and Jarndyce drones on. This scarecrow of a suit has, in course of time, become so complicated that no man alive knows what it means. The parties to it understand it least, but it has been observed that no two Chancery lawyers can talk about it for five minutes without coming to a total disagreement as to all the premises. Innumerable children have been born into the cause; innumerable young people have married into it; innumerable old people have died out of it. Scores of persons have deliriously found themselves made parties in Jarndyce and Jarndyce without knowing how or why; whole families have inherited legendary hatreds with the suit. The little plaintiff or defendant who was promised a new rocking-horse when Jarndyce and Jarndyce should be settled has grown up, possessed himself of a real horse, and trotted away into the other world. Fair wards of court have faded into mothers and grandmothers; a long procession of Chancellors has come in and gone out; the legion of bills in the suit have been transformed into mere bills of mortality; there are not three Jarndyces left upon the earth perhaps since old Tom Jarndyce in despair blew his brains out at a coffee-house in Chancery Lane; but Jarndyce and Jarndyce still drags its dreary length before the court, perennially hopeless.

epigraph-author: Charles Dickens

epigraph-source: Bleak House 

csl: casebook-bibliography.csl
bibliography: CivProCasebook.yaml

output:
  pdf_document:
    documentclass: tufte-book
    classoption: [sfsidenotes]
    filters:
      - include-files.lua
    toc: true
    toc-depth: 3
	number-sections: true
	number-depth: 2
    latex_engine: xelatex
    output-file: CivProBook_PDF
  commands: 
	small-size: small-size-command 
	center: center-command 
	center-icon: center-icon-command 
	center-icon-large: center-icon-large-command 
	mono-font: mono-font-command 
	sans-font: sans-font-command
---

# Frontmatter

Thanks everyone!

<!-- actual chapters start here -->

``` {.include}
chapters/introduction.md
chapters/methods.md
chapters/results.md
chapters/discussion.md
```

# Appendix

More info goes here.

``` {.include shift-heading-level-by=1}
// headings in included documents are shifted down a level,
// a level 1 heading becomes level 2.
appendix/questionaire.md
```