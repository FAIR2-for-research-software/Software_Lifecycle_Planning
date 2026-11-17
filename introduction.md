---
title: "Introduction"
teaching: 10
exercises: 2
---

:::::::::::::::::::::::::::::::::::::: questions

- How do we define software in research?
- What is the classical software lifecycle?
- What are the FAIR principles applied to research software?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Understand the definition of software in research.
- Understand the FAIR principles as applied to research software.
- Get to know (briefly) the software lifecycle.

::::::::::::::::::::::::::::::::::::::::::::::::

## What is a software in academia?

It is not always easy to define what constitutes software in a research setting. The size of projects can vary from a
small script of a few dozens of lines to a massive project with millions of lines. If you are interested in a discussion
around a research software definition a good starting point is [_Defining Research Software: a controversial
discussion_][defressoft]. An abbreviated summary of this paper and a pragmatic definition we use
as a basis for this course is...

::::::::::::::::::::::::::::::::::::: keypoints

Research Software includes source code files, algorithms, scripts, computational workflows and executables that were
created during the research process or for a research purpose. Software components (e.g., operating systems, libraries,
dependencies, packages, scripts,etc.) that are used for research but were not created during or with a clear research
intent should be considered software in research and not Research Software. This differentiation may vary between
disciplines.

::::::::::::::::::::::::::::::::::::::::::::::::

## Reminder: The FAIR principles applied to research software

The FAIR principles (Findable, Accessible, Interoperable and Reusable) were originally designed for research data in
order to "enhance their re-usability" (see [Wilkinson _et al_ (2016)][fair]). In this seminal paper it was made clear
that while data was a central aspect of research, the principles should also apply to algorithms, tools and workflows
that led to the production of that data. Few years later, in 2022, a set of recommendation was published ([Chue Hon _et
al._ (2022)][fair4rswg]; [Barker _et al._ (2022)][fair4rs]) in order to apply these FAIR principle to research
software. An overview of the FAIR principles adapted to research software are that...

::::::::::::::::::::::::::::::::::::: keypoints

- Findable: Software, and its associated metadata, is easy for both humans and machines to find.

- Accessible: Software, and its metadata, is retrievable via standardised protocols.

- Interoperable: Software interoperates with other software by exchanging data and/or metadata, and/or through
  interaction via Application Programming Interfaces (APIs), described through standards.

- Reusable: Software is both usable (can be executed) and reusable (can be understood, modified, built upon, or
  incorporated into other software).

::::::::::::::::::::::::::::::::::::::::::::::::

## The software lifecycle

A traditional software lifecycle (in a non-academic setup) involves the following phases:

![Traditional Software Lifecycle](fig/SLC.png){ width=50% }

1. **Requirements and Analysis**: Requirements are gathered from stakeholders (client, users) and analysed. From
  this, the Software Requirement Specification document is produced outlining all functional and non-functional
  requirements. The focus here is on understanding what the system is supposed to do without going into the details of
  implementation.

2. **System design**: The blueprint for building the system is created. It identifies the architecture, the
  components and their interaction but also focusing on the details of each components (data structure, databases,
  input/output).

3. **Development**: This is where the coding takes place. The developer will write the code based on the Software
  Requirement Specification to ensure that it meets requirements. It is often done iteratively by creating small
  building blocks.

4. **Integration and testing**: Once the code is written, the individual block are integrated to a complete system
  and various testing are conducted (e.g. unit tests, integration tests).

5. **Deployment**: Once the software is fully tested and ready, it is deployed to the production environment or
  delivered to the client. It is at this stage that the software is available to end-users.

6. **Maintenance**: At this stage, the software enters the maintenance phase where it is monitored, updated and fixed
  if necessary. Corrective maintenance fixes bugs, while adaptive and perfective maintenance improve the software's
  performance or add new functionalities.

It is quite a rigid framework that does not really adapt well to changes. This framework is often called a [waterfall
model][waterfall]. Nevertheless it is possible to adapt it to research the academic framework. That what we will see in
the software management plan in the next chapter.

[defressoft]: https://doi.org/10.5281/zenodo.5504016
[fair]: https://doi.org/10.1038/sdata.2016.18
[fair4rs]: https://doi.org/10.1038/s41597-022-01710-x
[fair4rswg]: https://10.5281/zenodo.5504015.
[waterfall]: https://en.wikipedia.org/wiki/Waterfall_model
