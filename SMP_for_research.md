---
title: "Software Managagement plan: Planning ahead"
teaching: 10
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions

- What should you ask yourself before starting a software project?
- How do I write a Software Management Plan?
- How do I disseminate my work and make it findable?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Understand the main points of a software management plan.
- Know the main questions you should ask yourself before diving into coding.

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

A Software Management Plan (SMP) is a framework that outlines how software development, releases, maintenance, and
support will be conducted throughout its lifecycle. It outlines how the key aspects like goals, resources, milestones,
risks, and quality are effectively controlled. The plan is usually created early in the project, ideally before work is
undertaken, and is essential for both small and large projects to ensure clear communication and expectations among team
members.

This chapter presents various point that you should think about when you start developing code for research. The goal is
that you ask yourself the right questions before embarking on your software development journey.

## Software Management Plan

Research is quite different from the private sector. The goal of a research software is to answer a research question in
a way that allows other people (and yourself) to carry it forward. Aligning the SMP to the research lifecycle ensures that
the software not only facilitates scientific progress but also meets academics standards for collaboration,
documentation and reproducibility.

### Project Overview

You will not start a research software project without having a research question you want to answer. Instead of business
requirement that you would have in a traditional software lifecycle you should therefore gather research
objectives. Having a clear research question will greatly help you define the requirements for your software.

But how do you proceed? The answer is the same as for the research question: you look at what is already out there in
the literature and software ecosystem of your domain. If someone has already answered your research question then you
typically  would not try to answer it again (unless seeking to replicate the finding). The same is true for research
software: you will first look at what is already available. The case where people are  re-implementing something that
already exist is far too common and wastes a lot of previous research time and funding. In short: **DO NOT RE-INVENT THE
WHEEL**. If something is already available but does not have all the functionalities you are looking for then maybe you
can build upon that previous work. If the code is open source, you might just be able to clone it and carry it forward
(as long as you give credit to the original author). Alternatively you may be able to contribute features up-stream to
the package you wish to use at the same time forging connections and potential collaborations. If it is not open source,
you might be able to contact the author and ask if you can have access to the source code, again this may lead to
fruitful collaborations!

If you still want to create something from scratch when something already exists, always ask yourself: what would make
people use my solution instead of the one that is already available? What benefits will my software bring to the
research community?

When you have a good sense of what you want to create you must define what data will be used as input and what the
output of the software will look like. It is common that for a given domain some data standard are already in use. Try
to stick to these standards as much as you can as doing so will make your software more **Interoperable** with other systems
and **Reusable** by others.

### Human and Technical resources

Once you have a good idea of what you want to create, the next step is to identify who is in charge of it. Identify team
members (e.g. P.I, Research Software Engineers (RSE), Postdocs, PhD students) and define their roles in the development
of the tool. It is often useful to extend the distribution of roles to other aspects of the project, such as data management
& publication (it is important that everybody gets credit for their work and **can evidence it**). Doing this before you
start you will help you identify what skills are available in your team and what, if any, deficiencies there are and
hence identifying the needs for training. Discussing these aspects beforehand will save you time and potentially help avoid
some painful discussions (and frustrations) down the line.

One crucial aspect of a software project, especially occurring in research, is the problem of the [bus
factor][busfactor]. Simply put it is a measurement of risk that arises if a member of the team were "_hit by a bus_" and
the information and capabilities they hold about the project has not been shared with the team.  The worst bus factor is
1 and means a single person is in charge of everything. If you lose that person then the project stops as no one else
knows about the project or has the skills to continue working on it. The higher the bus number the better as it means
there is shared knowledge and skills within the team. However, trying to mitigate this bus factor is crucial, and
sometimes very hard to do, particularly in smaller research groups. There are some steps that can be taken though, for
example you might want to have different people within the team familiar with the code. This can be achieved through
regular peer review during the development cycle. Perhaps most important is to have very clear and up-to-date
documentation on what the software does and how it is used.  The module on [Documentation][documentation] will be
helpful in how to go about this.

On the technical side, it is important to identify technical resources, e.g. computing environment, High Performance
Computing platform, that might be available. You might not see their need at first, but as development proceeds if
you know what support you can get from your own institution it will be useful know where and how accessible the support
is  as some, such as Research Software Engineer support, may need financing and you would need to plan this in advance
as part of the budget.

### Development Approach

How will you develop your code? Multiple ways exist to manage the development of a software, we can name two here:

- [Waterfall][waterfall]: This approach is a linear and sequential project management technique where each phase depends
  on the completion of the previous one. It consists of stages like requirements gathering, design, implementation,
  testing, deployment, and maintenance. Progress flows in one direction, similar to a waterfall. Changes are difficult to
  implement once a phase is completed. It is best suited for projects with well-defined requirements and minimal
  expected changes.

- [Agile][agile]: This approach is an iterative and flexible project management technique focused on delivering small,
  incremental improvements. It encourages collaboration between cross-functional teams, frequent feedback, and
  continuous adaptation to changes. Work is divided into short cycles called sprints, with regular reviews to assess
  progress. Agile prioritizes customer satisfaction through early and continuous delivery. It is best suited for dynamic
  projects with evolving requirements.

Whatever method of project management you choose, ensure that it is fostering collaboration within the group. Both have
their advantages but keep in mind that research is an iterative provess involving a lot of trial-and-error cycles and
experimentation. Communication will be a key aspect of success. It might be interesting to have short development
cycles with an iterative approach in which case an Agile approach would be more suited. This will help you analyse
intermediary research outcomes, review the development of the software (and documentation) and overall progress and
regularly review and realign the goals if necessary. It is not rare that while developing a research tool with a clear
goal in mind you end up finding serendipitous results that are worthy of publication in their own right!

The tools are you use for software development are also very important. Do not end up with multiple files for the multiple
version of your software (e.g. version1, version 1_1, version1_2, version1_final, version1_final2, etc.). It will
become unmanageable. To avoid this situation, it is important to have a version control tool that allows you to track
the changes that you implement in your software over time. Using version control will help making your software more
**FAIR**. If you are unfamiliar with version control then the modules on [Git for Beginners][gitzerohero] and
[Git Collaboration][gitcollaboration] will be useful.

### Timeline and Milestones

Creating software is not easy. The bigger it gets, the more complicated it becomes. Hence it is important to have
checkpoints, or milestones, that you can work toward. It is often possible to split the development of a software
package into multiple intermediary states. These intermediary states will give you more realistic and achievable
objectives and allow you to track progress and allow you to create your development timeline.

It is important to coordinate this timeline with research milestones and deadlines. They can be paper
submissions, conference presentations, funding deadlines, PhD thesis submissions. Software development and research
progress should be as aligned as possible and tracked concurrently. If they diverge you will be in trouble.

### Risk Management

**Spoiler alert: nothing will work from the first try!** You will inevitably encounter blockers which hinder progress
during the development of your software and only some of these will be identifiable beforehand. Failure to achieve
scientific outcomes, data issues (sometimes data will never arrive!), reproducibility failures, or tool/library
obsolescence are examples of risks that can be anticipated.

Once identified, you should think about how to mitigate these risks and create a contingency plan (a plan B) in case
they turn out to be real problems (e.g. backup strategies for data and code, alternative methods).

One important aspect of research it is that it is hard to plan. So how you address changes in the research hypothesis,
data, or experimental design and how this might impact software development is important to consider. Ensure proper
version control for both code and datasets and allow for flexibility for exploratory research where new insights might
lead to changes in the software. This gets much easier when the code is written in a maintainable, readable and
**Reusable** way. If unfamiliar with software development the module on [Design your code][codedesign] will be useful.

### Quality Assurance

Wouldn’t it be sad if all the work you have been putting in your software development is wasted by a typo in the code?
How do you make sure that the code you are writing is functioning as intended and that the scientific results your
producing are reliable and reproducible?

There are some strategies to ensure both code quality and research reproducibility:

- **Peer Review** : Code quality can be checked by doing code peer reviews. Regular peer review are very helpful both
  for increasing the quality and for disseminating knowledge in the team (reducing the bus factor). Automated testing
  with continuous integration. There are modules on [testing and continuous integration][pythontesting] and version
  control ([Git for Beginners][gitzerohero] and [Git Collaboration][gitcollaboration]) that can be undertaken.

- **Data Version Control** : Reproducibility will benefit from the previous suggestions, but you can also adopt a strategy
  for data version control (DVC) that will help track the state of your data and changes. Parametrisation of code
  ensures that it can be rerun with different parameters easily (without changing the code) via configuration files or
  command line interface. The module on [Code Design][codedesign] covers how to do this.

- **User Testing** : Testing by other people also helps. If someone else in your team can reproduce your results it will
  give you a good idea of how reproducible are your results. For a more advanced case, it is possible to fully
  automatise reproducibility checks and strategies for this are covered in the [testing and continuous
  integration][pythontesting] module.

- **Reliability** : The reliability of scientific output can be tested by comparing your code with existing
  datasets. Can you replicate existing results with your own tool? That will give you an interesting insight.

Tested software is more reliable and robust and thorough testing of your code will greatly enhance its **Re-usability**
and make your science more **Reproducible**.

### Dissemination

Dissemination is a cornerstone of research. When it comes to research software you will have to make sure that people
know where to find it and how to use it (**Findable** and **Reusable**). It comes down to three important pillars:

- **License**: This is probably one of the most basic items of the software management plan. If there is no license for
  your software people won't know if they have the right to reuse your software. No license means that you retain all
  the rights to your source code and no one may reproduce, distribute or create derivative works from your code (which is
  the opposite of research philosophy). Please see the chapter on intellectual property and software licenses for more
  details **[link TBD]**.

- **Documentation** is paramount, the main group that will help is your future self and members of your team! Research
  projects often span several years during which new members will join and some will leave the team. If it takes someone
  6 months just to understand the software that the team is developing that is wasted time. If you want a sustainable
  project, write good documentation. In addition, If you produce software with a good documentation it will be more
  likely used by the community and then you might get credit for it! Make sure that the documentation is easily
  accessible (e.g. a website) and tailored to future researchers and the academic community in your research domain. You
  should describe the research question the software seeks to solve as well as how the software works and should be
  used. The module on [Documentation][documentation] covers advice on how to document software projects.

- **Software Repositories**: It is important to place your software (the released version) to a place where people can
  download it freely. Collaborative development platform such as [Github][gh] and [GitLab][gl] are not made to store
  software on the long term. More persistent platforms designed for the sharing of research output exist such as
  [Figshare][figshare] and [Zenodo][zenodo] and should be used for long term storage of software. Please see chapter on
  dissemination for more details **[Link TBD]**.

To go a little bit further, you might want to take extra step in the dissemination direction:

- **Publication**: Once you release your software, you might want to publish it! Numerous journals accept papera about
  research software. Some are generalists (e.g. [JOSS][joss], JORS, [SoftwareX][softwarex] to name a few) and some are
  domain oriented (you can get a non-exhaustive list from the [Software Sustainability
  Institute][softwarepublishing])). A dedicated paper describing your software is really something you should consider!
  It will give you a lot of visibility and allow you to get a citable paper associated to your software (you can follow
  the lecture on [Publishing your software] for this).

- **Training**: If your software sees a lot of buy-in from the community and is relatively complex to use (not all
  software is), you might want to train others to use it. You can do that via tutorials and/or training events. This is
  a very powerful way to give your work more visibility and a very efficient way to create collaborations!

### Long term sustainability

Maintenance of the software is tricky. There are two possible scenarios:

- The software is in a final form, but the funding is still there: In that case it is important to identify who is in
  charge of the maintenance and update. You might be working with totally different people than at the beginning of the
  project. So it is important to plan ahead for this in the Software Management Plan.

- The research project comes to an end (and with it, its founding). That’s the tricky situation, long term maintenance
  is difficult because funders do not plan for this (which happens everywhere). If you want to increase the chances
  that your software works in 5 or 10 years, what you could envisage to do is to distribute your software with its own
  computational environment. This ships your software with the required dependencies and put all this in its own
  bubble. This greatly enhances the long term **Reproducibility** of your work. If you are interested to learn more about
  this, you can enrol in the [Reproducible Computational Environment][reprocompenv].

In either scenario having accessible and detailed documentation will be really useful for the long term maintenance of
the code.

## Minimal version

Everything that has been described previously can be quite intimidating at first. There is a lot to think about and
depending on the size of your project you might not need all of these details. If you want to go with a minimal set of
items to put in place you could use the following:

1. Information on what software outputs (including documentation and other related material) are expected to be
   produced.
2. Who is responsible for the development work?;
3. Which version control system is to be used?
4. What license will be used for each produced piece of code/data?

These four items should be on your list in the planning phase.

[agile]: https://en.wikipedia.org/wiki/Agile_software_development
[busfactor]: https://en.wikipedia.org/wiki/Bus_factor
[codedesign]: https://romain-thomas-shef.github.io/FAIR_Code_design/
[documentation]: https://joe-heffer-shef.github.io/FAIR4RS-Documentation/
[figshare]: https://figshare.com/
[gh]: https://github.com/
[gl]: https://gitlab.com/
[gitzerohero]: https://srse-git-github-zero2hero.netlify.app/
[gitcollaboration]: https://blog.nshephard.dev/git-collaboration/
[joss]: https://joss.theoj.org/
[pythontesting]: https://sylviawhittle.github.io/python-testing-for-research/
[reprocompenv]: https://ubdbra001.github.io/FAIR4RS-VirtualEnvs/
[softwarepublishing]: https://www.software.ac.uk/top-tip/which-journals-should-i-publish-my-software
[softwarex]: https://www.sciencedirect.com/journal/softwarex
[waterfall]: https://en.wikipedia.org/wiki/Water_model
[zenodo]: https://zeondo.org
