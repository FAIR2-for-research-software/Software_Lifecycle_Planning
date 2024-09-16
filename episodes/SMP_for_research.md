---
title: "Software Managagement plan: Planning ahead"
teaching: 10
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions 

- What should you ask yourself before starting a software project?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Understand what are the main points of a software management plan
- How does it adapt to your research?

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction


## A traditional Software Management Plan (SMP)


## The version adapted for research

Research is quite different from private sector. The goal of a research software is to answer a research question in a way that allows other people (and yourself) to carry it forward. ALigning the SMP to the research lifecyle ensure that the software not only facilitates scientific progress but also meets academics standards for collaboration, documentation and reproducibility.

Note: Not covered here is the finance part of the plan.. 


### Project Overview

This is the start of the project. You will not start a research software without having a research question you want to answer. Having a clear research question will greatly help you define your software. 

Then what would you do? The answer is the same as for the research question: you look at what is already out there in the literature. If someone already answered your research question then you would not try to answer it again. So if you want to build a software you will first look at what is already available. **DO NOT RE-INVENT THE WHEEL**. 
If something similar exists then don't recode it! If something is already available but does not have all the functionalities you are looking for then maybe you can build upon that previous work. If the code is open source, you might just be able to clone it and carry it forward. If it is not, you might be able to contact the P.I. and ask if you can have access to the source code (you might create new collaborations!). 

If you still want to create something from scratch while something already exist, always ask yourself: what would make people use my solution intead of the one that is already there? What addition do my software add to research community?

### Human and Technical ressouces

Once you have a good idea of what you want to create, the next step is to identify who is in charge of it. Identify team members (P.I, RSE, Postdoc, PhD student, Data scientist) and their roles in the development of the tool. It is often useful to extend these distribution of roles to other aspects of the project, such as data management & publication (scienctif onces and more technical ones). Not everybody has the same role nor the same interests so the distribution of roles is crucial. It is also important to make sure that everbody gets credited when the work is done. Discussing these aspects beforehand will potentialy avoid some painfuly difficult discussion (and frustration) down the line.  

On the technical side, it is important to identify technical resources, e.g. computing environement, High Performance Computing platform, that might be available. You might not see their need at first, but as the development goes on, if you know what support you can get from your own institution it is always interesting to know where they are and how accessible they are (some might need financing!). 

* Focus: Define responsibilities not just for coding, but also for research integrity, data handling, and ensuring reproducibility.


### Development Approach

How will you develop your code? Multiple ways exist to manage the development of a software, we can name two here:

* Waterfall:

* Agile:


Research is an iterative provess involving a lot of trials/errors cycle and experimentation and communication will be a key aspect of success. It might be interesting to have short development cycles with an iterative approach. This will help you analyse intermediary research outcomes, review the development of the software (and documentation) and overall progress. It is not rare that while developing a research tool with a clear goal in mind you end up finding serendipitous results. Whatever method of project management you choose, ensure that it is fostering collaboration within the group. 

In addition, what tools are you using for software development? Do not end up with multiple files for the multiple version of your software (e.g. version1, version 1_1, version1_2, version1_final, version1_final2, etccc). It will become unmanageable. To avoid such a situationm, it is important to have a version control tool that allows you to track the changes that you implement in your software. **[Add link to Neil's lectures]** 

### Timeline and Milestones

Creating a software is not easy. The bigger it gets, the more complicated it becomes. Hence it is important to have checkpoints, or milestones, that you can work toward. It is often possible to split the development of a research into multiple intermediary states. These intermediary states will give you a more achievable work and allow you to track the work. This will create your development timeline. 

In addition, it is important to coordinate this timeline with research milestones and deadlines. They can be paper submissions, conference presentations, funding milestones, PhD thesis milestones. Software development and research progress might be aligned and tracked concurently. If they diverge you will be in trouble.  


### Risk Management

**Nothing will work from the 1st try!** You will find blockades on the way and some can be identified beforehand. Failure to achieve scientific outcomes, data issues (sometimes will never come!), reproducibility failures, or tool/library obsolescence are example of such risks.

Once identified, you should think how to mitigate these risks and create a contingency plan (plan B) in case they turn out to be real problems (e.g., backup strategies for data and code, alternative methods).

One important aspect of research it is that it is hard to plan. So how will you address changes in the research hypothesis, data, or experimental design and how might that impact the software. Ensure proper version control for both code and datasets and allow for flexibility for exploratory research where new insights might lead to changes in the software. This gets much easier when the code is written in a maintainable and readable way **(cf lecture on code design by R. Thoma, [add link to lecture]).


## Minimal version



