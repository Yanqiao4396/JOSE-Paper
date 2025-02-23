---
title: 'Using Treesitter-Based Techniques to Automatically Detect Code Smells in Programming Projects'
tags:
  - code quality
  - code smell
  - python
  - java
  - javascript
authors:
  - name: Yanqiao Chen
    orcid: 0000-0003-0872-7098
    affiliation: "1, 2" # (Multiple affiliations must be quoted)
  - name: Author Without ORCID
    affiliation: 2
affiliations:
 - name: Lyman Spitzer, Jr. Fellow, Princeton University
   index: 1
 - name: Institution 2
   index: 2
date: 16 February 2025
bibliography: paper.bib

# Optional fields if submitting to a AAS journal too, see this blog post:
# https://blog.joss.theoj.org/2018/12/a-new-collaboration-with-aas-publishing
aas-doi: 10.3847/xxxxx <- update this with the DOI from AAS once you know it.
aas-journal: Astrophysical Journal <- The name of the AAS journal.
---

# Summary

TreeNose is a language-independent static analysis tool for detecting code smells, a series of code-design-related concerns that may decrease readability and maintainability of software projects. Meanwhile, one of the characteristics of modern Computer Science education is the learning of different programming languages in multiple or even single courses. TreeNose helps instructors to design code smells detectors in different programming languages under the same rules used to track code smells from assignments, therefore avoiding the nuance of configuring multiple language-specific detectors. TreeNose features the implementation of Treesitter, a general parser generator, which provides users a easy and universal configuration experience in different programming languages for instructors and an universal detection experience for student. By default, TreeNose supports 5 common code smells: Long Method, Long Class, Long Parameter List, Complex Conditional, Long Message Chain and 3 programming languages: Java, JavaScript and Python.

# Statement of Need

Code smells are a series of code-design-related concerns
that may decrease readability and maintainability of software projects, ultimately limiting opportunities for future maintenance. One of the characteristics of many modern software projects is their use of multiple programming languages. The
combination of programming languages allows developers to
mix and match the functionalities and libraries that are best
supported by a specific programming language. While developers noticed the harm of code smells in projects and built a series of code smell detectors, most of code smell detectors are language-specific. Therefore, developers usually apply a combination of code smell detectors for the multi-language projects, thereby introducing the burdensome
need to consistently configure multiple smell detection tools. This nuance also affects instructors in the modern Computer Science courses. Research shows instructors over the world apply different programming languages or combination of them in the introductory cs courses. Industry-prevalent Programming languages like Python and Java are widely used in Computer Science courses. At the same time, researchers prove that, by applying static analysis tools like Pylint, instructors can effectively track students’ understanding in coding best practices in an introductory cs course of 200 students

Since the debut of LLM, surveys show Generative Artificial Intelligence (GenAI), like Codex and Copilot, are widely used by students when working with code. However, those GenAIs have the tendency to contain code smell problems because of inherent code smells from their source database. Therefore, TreeNose can also help students to identify those code smells in the AI generated code that they may apply but fail to evaluate.


# Citations

Citations to entries in paper.bib should be in
[rMarkdown](http://rmarkdown.rstudio.com/authoring_bibliographies_and_citations.html)
format.

For a quick reference, the following citation commands can be used:
- `@author:2001`  ->  "Author et al. (2001)"
- `[@author:2001]` -> "(Author et al., 2001)"
- `[@author1:2001; @author2:2001]` -> "(Author1 et al., 2001; Author2 et al., 2002)"

# Figures

Figures can be included like this: ![Example figure.](figure.png)

# Acknowledgements

We acknowledge contributions from Brigitta Sipocz, Syrtis Major, and Semyeong
Oh, and support from Kathryn Johnston during the genesis of this project.

# References