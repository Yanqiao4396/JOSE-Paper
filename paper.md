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
  - name: pass # TODO: Add your name here
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

TreeNose is a language-independent static analysis tool for detecting code smells,
a series of code-design-related concerns. One of the characteristics of modern Computer
Science education is the learning of different programming languages. While the code smells
in programming languages are language-independent, the detectors aren't. Therefore, applying multiple
code smell detectors and configuring them in a single multi-language project is a burdensome procedure.
To overcome this challenge, TreeNose helps instructors to design code smells detectors 
in different programming languages under consistent detection rules. Such a multi-language code smell detector
can help to track code smells residing in assignment projects of students, avoiding the nuance of 
configuring multiple language-specific detectors. TreeNose features the implementation 
of Treesitter, a general parser generator, which provides users a easy and 
universal configuration experience in different programming languages. 
By default, TreeNose supports 5 of the most common code [@developersCare] smells:
Long Method, Long Class, Long Parameter List, Complex Conditional, Long Message Chain 
in 3 programming languages: Java, JavaScript and Python. Among 3 languages we support, 
Java and Python widely widely implemented in the introductory Computer Science courses 
[@introProgrammingSurvey], and JavaScript is one of the mostly widely used programming 
languages in the industry [@StackOverflowSurvey].

# Statement of Need

Code smells are a series of code-design-related concerns
that may decrease readability and maintainability of software projects, 
ultimately limiting opportunities for future maintenance. 
One of the characteristics of many modern software projects is their use of 
multiple programming languages[@723183]. The combination of programming languages allows
developers to mix and match the functionalities and libraries that are best 
supported by a specific programming language. While developers noticed the harm of 
code smells in projects and built a series of code smell
detectors, most of code smell detectors are language-specific. 
Therefore, developers usually apply a combination of code smell detectors for the 
multi-language projects, thereby introducing the burdensome
need to consistently configure multiple smell detection tools. 
This nuance also affects instructors in the modern Computer Science courses.
Researchers prove that, by applying static analysis tools like Pylint, 
instructors can effectively track students’ understanding in coding best practices 
in an introductory cs course [@usingStaticAnalysisTools].
On the another side of the spectrum, there exists a trend worldwide where instructors
apply different programming languages or combination of them in the introductory cs courses. 
Industry-prevalent programming languages like Python and Java are widely used in Computer Science courses [@introProgrammingSurvey].
For professors who would like to apply code smell detectors and instruct courses interacting with multiple programming languages
, they can't avoid the problem of applying multiple language specific code smell detectors.
However, due to the fact that different code smell detectors have different
detection rules and audience code smells, the combination of language-specific code smell detectors
hardly cover the detection of certain code smells in all the supported languages under the aligned detection rules.

Since the debut of LLM, surveys show Generative Artificial Intelligence (GenAI), like Codex and Copilot, 
are widely used and accepted by students when working with code [@robotInEducation]. However, those GenAIs have the tendency to contain code smell problems because of inherent code smells from their source database[@codeSmellInGenAI]. Therefore, TreeNose can also help students to identify those code smells in the AI generated code that they may apply but fail to evaluate first.

# Applications of TreeNose

TODO: Application of TreeNose in Menagerie, an open source scored assignment dataset [@messer_brown_kölling_shi_2024]

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


# References