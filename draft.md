## Statement of Need
Colleges these years apply multiple programming languages in the courses (include introductory courses) [reference1](https://dl.acm.org/doi/pdf/10.1145/3626252.3630761). Industry-prevalent Programming languages like Python and Java are widely used in Computer Science courses. At the same time, researchers prove that, by applying static analysis tools like Pylint instructors can effectively track students’ understanding in coding best practices in an introductory cs course of 200 students [reference2](https://dl.acm.org/doi/pdf/10.1145/3626252.3630761)

By combining those two ideas, we believe it's valuable to apply detection within multi-languages to code smells, Code smells are a series of code-design-related concerns that may decrease readability and maintainability of software projects.
we believe a multi-language code smell detector can help instructors to track students’ understanding of code smells in multiple languages across courses. To resolve this gap, we built TreeNose, a customizable multi-language code smells detector. TreeNose implements universal rules, making it highly configurable and extendable, thanks to the implementation of Treesitter, a general parser generator. TreeNose provides aligned configuration and detection experiences in different programming languages for instructors students.

Since the debut of LLM, surveys show Generative Artificial Intelligence (GenAI), like Codex and Copilot, are widely used by students when working with code [reference 3](https://dl.acm.org/doi/pdf/10.1145/3623762.3633499). However, those GenAIs have the tendency to contain code smell problems because of inherent code smells from their source database [reference 4](https://s2e-lab.github.io/preprints/scam22-preprint.pdf). Therefore, TreeNose can also help students to identify those code smells in the AI generated code that they may apply but fail to evaluate.

## Summary
- The architecture of TreeNose
- Code smells supported by TreeNose
- Language configuration example with TreeNose
- Shallow summary of the F1 score result from the experiments done by us

## Use Case
- Applying TreeNose as a part of automated static analysis code quality checking chain in students’ code assignments
- Benefit students to be aware of code smell and code quality
- Benefit professors to notice students’ performances on code smells
