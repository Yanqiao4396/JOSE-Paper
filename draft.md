## Statement of Need
Colleges apply multiple programming languages in the courses (include introductory courses) [reference1](https://dl.acm.org/doi/pdf/10.1145/3626252.3630761)

Researcher proves applying static analysis tools like Pylint can effectively monitor students’ understanding in coding best practices in an introductory cs course of 200 students [reference2](https://dl.acm.org/doi/pdf/10.1145/3626252.3630761)

By combining those two ideas, we believe a multi-language code smell detector can help instructors to monitor students’ performances in multiple languages across courses
What makes our tool different is that TreeNose implements universal rules, and is highly configurable and extendable  thanks to the implementation of Treesitter, allowing instructors and students to have aligned configuration and detection rules across programming languages

Since the debut of LLM, surveys show GenAIs, like Codex and Copilot, are widely used by students when working with code [reference 3](https://dl.acm.org/doi/pdf/10.1145/3623762.3633499). However, those GenAI has the tendency to contain code smell problems because of their source database [reference 4](https://s2e-lab.github.io/preprints/scam22-preprint.pdf). Code smell detectors can assist to identify those code smells from GenAI 

## Summary
- The architecture of TreeNose
- Code smells supported by TreeNose
- Language configuration example with TreeNose
- Shallow summary of the F1 score result from the experiments done by us

## Use Case
- Applying TreeNose as a part of automated static analysis code quality checking chain in students’ code assignments
- Benefit students to be aware of code smell and code quality
- Benefit professors to notice students’ performances on code smells
