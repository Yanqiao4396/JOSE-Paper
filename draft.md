## Summary
- What is code smell and why it matters (especially for students and instructors)
- The language-independence of code smells
- How TreeNose can help
- Main future of TreeNose (1. Language support 2. Code smell support)
- The architecture of TreeNose
- Shallow summary of the F1 score result from the experiments done by us

TreeNose is a language-independent static analysis tool for detecting code smells, a series of code-design-related concerns that may decrease readability and maintainability of software projects. Meanwhile, one of the characteristics of modern Computer Science education is the learning of different programming languages in multiple or even single courses. TreeNose helps instructors to design code smells detectors in different programming languages under the same rules used to track code smells from assignments, therefore avoiding the nuance of configuring multiple language-specific detectors. TreeNose features the implementation of Treesitter, a general parser generator, which provides users a easy and universal configuration experience in different programming languages for instructors and an universal detection experience for student. By default, TreeNose supports 5 common code smells: Long Method, Long Class, Long Parameter List, Complex Conditional, Long Message Chain and 3 programming languages: Java, JavaScript and Python.


## Statement of Need

Code smells are a series of code-design-related concerns
that may decrease readability and maintainability of software projects, ultimately limiting opportunities for future maintenance. One of the characteristics of many modern software projects is their use of multiple programming languages. The
combination of programming languages allows developers to
mix and match the functionalities and libraries that are best
supported by a specific programming language. While developers noticed the harm of code smells in projects and built a series of code smell detectors, most of code smell detectors are language-specific. Therefore, developers usually apply a combination of code smell detectors for the multi-language projects, thereby introducing the burdensome
need to consistently configure multiple smell detection tools. This nuance also affects instructors in the modern Computer Science courses. Research shows instructors over the world apply different programming languages or combination of them in the introductory cs courses [reference1](https://dl.acm.org/doi/pdf/10.1145/3626252.3630761). Industry-prevalent Programming languages like Python and Java are widely used in Computer Science courses. At the same time, researchers prove that, by applying static analysis tools like Pylint, instructors can effectively track students’ understanding in coding best practices in an introductory cs course of 200 students [reference2](https://dl.acm.org/doi/pdf/10.1145/3412453.3423195)

Since the debut of LLM, surveys show Generative Artificial Intelligence (GenAI), like Codex and Copilot, are widely used by students when working with code [reference 3](https://dl.acm.org/doi/pdf/10.1145/3623762.3633499). However, those GenAIs have the tendency to contain code smell problems because of inherent code smells from their source database [reference 4](https://s2e-lab.github.io/preprints/scam22-preprint.pdf). Therefore, TreeNose can also help students to identify those code smells in the AI generated code that they may apply but fail to evaluate.


## Use Case
- Applying TreeNose as a part of automated static analysis code quality checking chain in students’ code assignments
- Benefit students to be aware of code smell and code quality
- Benefit professors to notice students’ performances on code smells
