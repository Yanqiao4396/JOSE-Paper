## Summary
- What is code smell and why it matters (especially for students and instructors)
- The language-independence of code smells
- How TreeNose can help
- Main future of TreeNose (1. Language support 2. Code smell support)
- The architecture of TreeNose
- Shallow summary of the F1 score result from the experiments done by us

Code smells are a series of code-design-related concerns
that may decrease readability and maintainability of software projects, ultimately limiting opportunities for future maintenance. One of the characteristics of many modern software projects is their use of multiple programming languages. The
combination of programming languages allows developers to
mix and match the functionalities and libraries that are best
supported by a specific programming language. While developers noticed the harm of code smells in projects and built a series of code smell detectors, most of code smell detectors are language-specific. Therefore, developers usually apply a combination of code smell detectors for the multi-language projects, thereby introducing the burdensome
need to consistently configure multiple smell detection tools. This nuance also affects instructors in the modern Computer Science courses. Research shows instructors over the world apply different programming languages or combination of them in the introductory cs courses [reference1](https://dl.acm.org/doi/pdf/10.1145/3626252.3630761). At the same time, researchers prove that, by applying static analysis tools like Pylint, instructors can effectively track students’ understanding.

TODO: rest of them are in statement of need. I have a hard time to distinguish the rest of summary and statement of need....

## Statement of Need
Colleges these years apply multiple programming languages in the courses (include introductory courses) [reference1](https://dl.acm.org/doi/pdf/10.1145/3626252.3630761). Industry-prevalent Programming languages like Python and Java are widely used in Computer Science courses. At the same time, researchers prove that, by applying static analysis tools like Pylint, instructors can effectively track students’ understanding in coding best practices in an introductory cs course of 200 students [reference2](https://dl.acm.org/doi/pdf/10.1145/3412453.3423195)

By combining those two ideas, we believe it's valuable to apply detection within multi-languages to code smells, Code smells are a series of code-design-related concerns that may decrease readability and maintainability of software projects.
we believe a multi-language code smell detector can help instructors to track students’ understanding of code smells in multiple languages across courses. To resolve this gap, we built TreeNose, a customizable multi-language code smells detector. TreeNose implements universal rules, making it highly configurable and extendable, thanks to the implementation of Treesitter, a general parser generator. TreeNose provides aligned configuration and detection experiences in different programming languages for instructors students.

Since the debut of LLM, surveys show Generative Artificial Intelligence (GenAI), like Codex and Copilot, are widely used by students when working with code [reference 3](https://dl.acm.org/doi/pdf/10.1145/3623762.3633499). However, those GenAIs have the tendency to contain code smell problems because of inherent code smells from their source database [reference 4](https://s2e-lab.github.io/preprints/scam22-preprint.pdf). Therefore, TreeNose can also help students to identify those code smells in the AI generated code that they may apply but fail to evaluate.


## Use Case
- Applying TreeNose as a part of automated static analysis code quality checking chain in students’ code assignments
- Benefit students to be aware of code smell and code quality
- Benefit professors to notice students’ performances on code smells
