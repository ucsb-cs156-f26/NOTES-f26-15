# Section 4.6: How Big: Small vs. Large Codebases

Summary by Roland C. 

# Question 1

My experience is a mix, but it mostly lines up with what the interview subjects reported. School has given me some exposure to existing code, but almost never at the scale, or with the messiness, that I ran into working in industry.

Where my experience matches the paper
Most school work has been small and stand-alone. In most of my CS courses (networking, security, AI, or even competitive programming), I wrote programs more or less from scratch, or with skeleton files. These were usually one or a few files, and the main goal was to get the right output. Like P08 said, it was easy to "overflow one file" with everything, since nobody would ever read or extend it after it was graded.
Industry was mostly reading code, not writing it. One of my projects I worked on was to design a config-driven parser to replace a set of tool-specific Java log parsers. Before I could write anything new, I spent weeks tracing how the existing system worked, from a .properties file through a parser manager down to a 1,000+ line parser class. Some of it I only had as decompiled bytecode. This is exactly what P04 described: you have to understand the system before you can design something that builds on top of it and also P06's wish for more practice "reading code and working in other codebases" really resonates with me.
Where my experience differs
School did give me some practice working inside provided code. In some classes, such as my computer architecture labs in PyRTL and an operating systems assignment implementing a FAT-style file system, we were handed starter code and had to work within its structure and constraints. So I wasn't starting completely from zero the way some participants described.
However, that starter code was small and clean. It was written to be understood by students. That is very different from a large, undocumented production codebase with years of accumulated hacks, where the original authors are gone.

# Question 2

Regarding the size and scale of codebases, developers interviewed in the paper found several aspects of industry practice surprising or different compared to school:

* **Working in Large Existing Codebases:** Developers found that in industry, they spend significantly more time reading code and adding features to massive existing codebases rather than building stand-alone programs from scratch.
* **The Critical Role of Refactoring and Design:** Participants were surprised by the importance of architectural design, refactoring, and single-responsibility principles compared to academic settings, where code is often thrown into a single file just to get the task done.
* **Strict Code Style Standards:** Developers noted how strict style guides and disciplined code structuring are required in industry—not just for grading, but because developers code so rapidly that clear style is necessary to understand their own and others' past work.

# Question 3

To better prepare students for working with large codebases as practiced in industry, we can try to implement some of these

1. **Practice reading and extending existing systems:** Computer science curricula should provide pre-built frameworks where students must read and understand the existing code before building new features on top of it.
2. **Emphasize refactoring, design principles, and library integration:** Courses should teach refactoring and architectural principles (like single responsibility) so students learn to break down monolithic code, as well as give practice integrating external libraries into projects.
3. Enforce clean code practices and or possibly utilize linting early in projects
