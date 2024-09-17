---
title: "Software Managagement plan: Planning ahead"
teaching: 10
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions 

- What should you ask yourself before starting a software project?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Understand what are the main points of a software management plan.
- What are they main question you should ask yourself before diving into the coding part.

::::::::::::::::::::::::::::::::::::::::::::::::

## Introduction

A Software management plan [SMP] is a framework that outlines how software development, releases, maintenance, and support will be conducted throughout its lifecycle. It outlines how the key aspects like goals, ressources, milestone, risks, and quality are effectively controlled. The plan is usually created early in the project and is essential for both small and large projects to ensure clear communication and expectations among team members and stakeholders. In this chapter we present various point that you might want to think about when you start developing a code for research. The goal is that you ask yourself the right questions before embarking in an important software development journey. 

## Software management plan in academia

Research is quite different from private sector. The goal of a research software is to answer a research question in a way that allows other people (and yourself) to carry it forward. Aligning the SMP to the research lifecyle ensure that the software not only facilitates scientific progress but also meets academics standards for collaboration, documentation and reproducibility.

### Project Overview

This is the start of the project. You will not start a research software without having a research question you want to answer. Having a clear research question will greatly help you define your software. 

Then what would you do? The answer is the same as for the research question: you look at what is already out there in the literature. If someone had already answered your research question then you would not try to answer it again. So if you want to build a software you will first look at what is already available. **DO NOT RE-INVENT THE WHEEL**. 

If something similar exists then don't recode it! If something is already available but does not have all the functionalities you are looking for then maybe you can build upon that previous work. If the code is open source, you might just be able to clone it and carry it forward. If it is not, you might be able to contact the P.I. and ask if you can have access to the source code (you might create new collaborations!). 

If you still want to create something from scratch while something already exists, always ask yourself: what would make people use my solution intead of the one that is already available? What addition does my software bring to the research community?

Finally, what do you expect to produce? What is the end product?  What output will it create? How will I make people engage with it?  All these questions are important!

### Human and Technical ressouces

Once you have a good idea of what you want to create, the next step is to identify who is in charge of it. Identify team members (P.I, RSE, Postdocs, PhD students) and their roles in the development of the tool. It is often useful to extend these distribution of roles to other aspects of the project, such as data management & publication (scientific and more technical ones). Discussing these aspects beforehand will potentialy avoid some painfuly difficult discussion (and frustration) down the line.  

One crucial aspect of a software project, especially occuring in research, is the problem of the bus factor. Simply put the bus factor is a number equal to the amount of people in your project that could get it by a bus without putting your project in trouble. The worst bus factor is 1 and means a single person is in charge of everything. If you lose that person that project stops. Trying to mitigate this bus factor is crucial, and sometimes very hard to do. You might want to have different people aware of the code(through peer code review in the team), and what will be very important is to have a very clean and up-to-date documentation (the lecture on [Documentation] might help you do that). Finally, It is also important to make sure that everbody gets credited for their work. 

On the technical side, it is important to identify technical resources, e.g. computing environement, High Performance Computing platform, that might be available. You might not see their need at first, but as the development goes on, if you know what support you can get from your own institution it is always interesting to know where they are and how accessible they are (some might need financing!). 

### Development Approach

How will you develop your code? Multiple ways exist to manage the development of a software, we can name two here:

* Waterfall: **TBD**

* Agile: **TBD**

Whatever method of project management you choose, ensure that it is fostering collaboration within the group. Research is an iterative provess involving a lot of trials/errors cycle and experimentations. Communication will be a key aspect of success. It might be interesting to have short development cycles with an iterative approach. This will help you analyse intermediary research outcomes, review the development of the software (and documentation) and overall progress. It is not rare that while developing a research tool with a clear goal in mind you end up finding serendipitous results that are worth a publication! 

In addition, what tools are you using for software development? Do not end up with multiple files for the multiple version of your software (e.g. version1, version 1_1, version1_2, version1_final, version1_final2, etccc). It will become unmanageable. To avoid such a situation, it is important to have a version control tool that allows you to track the changes that you implement in your software (Program lectures on this topic: [Git-beginners] & [Git-collab].

### Timeline and Milestones

Creating a software is not easy. The bigger it gets, the more complicated it becomes. Hence it is important to have checkpoints, or milestones, that you can work toward. It is often possible to split the development of a research into multiple intermediary states. These intermediary states will give you more realistic and achievable objectives and allow you to track the work. This will create your development timeline. 

In addition, it is important to coordinate this timeline with research milestones and deadlines. They can be paper submissions, conference presentations, funding milestones, PhD thesis milestones. Software development and research progress should be as aligned as possible and tracked concurently. If they diverge you will be in trouble.  

### Risk Management

**Nothing will work from the first try!** You will find blockades on the way and some can be identified beforehand. Failure to achieve scientific outcomes, data issues (sometimes will never come!), reproducibility failures, or tool/library obsolescence are example of such risks.

Once identified, you should think how to mitigate these risks and create a contingency plan (a plan B) in case they turn out to be real problems (e.g., backup strategies for data and code, alternative methods).

One important aspect of research it is that it is hard to plan. So how will you address changes in the research hypothesis, data, or experimental design and how might that impact the software. Ensure proper version control for both code and datasets and allow for flexibility for exploratory research where new insights might lead to changes in the software. This gets much easier when the code is written in a maintainable and readable way (The lecture on [Design your code] might be helpful for this).


### Quality Assurance

*Wouldn’t it be sad that all the work you have been putting in your software development is wasted by a typo in the code?* How do you make sure that the code you are writing is doing things as it is intended to be done? And that the scientific results your producing are reliable and reproducible?  

Develop strategies to ensure both code quality and research reproducibility:
* The code quality can be achieved by doing code peer reviews. Regular peer review are very helpful both for increasing the quality and for disseminating knowledge in the team (reducing the bus factor). Automated testing with continuous integration (cf lecture on Testing and continuous integration with S. Wittle **[link TBD]**), version control (cf LectureS on version control by Neil Shepherd **[link TBD]**), etc… 
* Research reproducibility will also benefit from all of the previous suggestions, but you can add data version control (DVC) that will help track the state of your data and changes, parametrisation of code ensures that it can be rerun with different parameters easily (without changing the code) via configuration files or command line interface **[link TBD]**.  Testing by other people also helps. If someone else in your team can reproduce your results gives a good idea of how reproducible are your results. Finally, and for a more advanced case, it is possible to fully automatise reproducibility checks.  

* Reliability of science results can be tested by comparing your code with exsiting datasets. Can you replicate exiting results with your own tool? That will give you an interesting insight. 


### Dissemination.

Dissemination is a cornerstone of research. When it comes to research software you will have to make sure that people know where to find it and how to use it. It comes down to three important pilars:

* License: This is probably one of the most basic item of the software management plan. If there is no license in your software people won't know if they have the right to re-use your software. No license means that you retain all the rights to your source code and no one may reproduce, distribute or create derivative works from your code (which is the opposite of research philosophy). Please see the chapter on intellectual property and software licenses for more details **[link TBD]**.

* Documentation is paramount: And guess what, the main group that it will help is YOUR TEAM! Research projects often span several years with people coming in and some leaving the team. If it takes someone 6 months just to understand the software that the team is developing it is going to be a waste of time. If you want a sustainable project, write a good documentation. In addition, If you produce a software with a good documentation it will be more likely used by the community and then you might get credit for it! You should make sure that the documentation is easily accessible (e.g. a website) and tailored to future researchers and the academic community in your research domain (cf Documentation module with Joe Heffer **[link TBD]**). Document how the software works, but not only this. Always describe how it serves a research question. 

* Software repositories: It is important to place your software (the released version) to a place where people can download it freely. Collaborative development platform such as github are not made to store software on the long term. Nevertheless, other platform are made for this (e.g. figshare, zenodo, etc..). This is where you should look for a long term storage. Please see chapter on dissemination for more details **[Link TBD]**.

To go a little bit further, you might want to take extra step in the dissemination direction:

* Publication: Once you release your software, you might want to publish it! Numerous journals accept papera about research software. Some are generalists (e.g. JOSS, JORS, SoftwareX, etc **[add links]**) and some are domain oriented **[add link TBD]**. This is really something you should consider! It will give you a lot of visibility and allow you to get a citable paper associated to your software [**link to JOSS lecture**].

* Training: If your software sees a lot of buy-in in the community and that is relatively complex to use (not all software are), you might want to train others to use it. You can do that via tutorials or training events. This is a very powerful way to give your work more visibility and a very efficient way to create collaborations!



### Long term sustainability
Maintenance of the software is tricky. We can distinguish two parts: 
- The software is in a final form, but the founding is still there: In that case it is important to identify who is in charge of the maintenance and update. You might work with totally different people than at the beginning of the project. So it is important to plan this ahead (cf previous section). A good documentation will always help the maintenance.
- The research project comes to an end (and with it, its founding). That’s the tricky situation, long term maintenance is difficult because founders do not plan for this (which happens everywhere).  If you want to increase the chance that your software work in 5 or 10 years, what you could envisage to do is to distribute your software with its own computational environment. This ships your software with the required dependencies and put all this in its own bubble.  If you are interested to learn more about this, register to the lecture on reproducible Computational environment, by Daniel Brady **[Link TBD]**.

In general, making a software open-source, will increase the chance that other people can increase its lifetime beyond your own involvement! (Cf section on Software Licence)

## Minimal version

Everything that has been described previously can be quite intimidating at first. There is a lot to think about and depending on the size of your project you might not need all of these details. If you want to go with a minimal set of items to put in place you could choose the following ones:

* Information on what software outputs (including documentation and other related material) are expected to be produced ; 
* Who is responsible for the development work?;
* The version control process to be used;
* What license will be used for each output?

These four items should be mandatory for each software created in academia. 


