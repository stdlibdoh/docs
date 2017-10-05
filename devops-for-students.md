# DevOps for students

## Target Audience

Any student interested in doing group work, be it for personal projects or even university related coursework.

## Introduction

Following are the notes accompanying my presentation on "DevOps for students", given during [Doc.Hack (2017)](http://goldsmiths.tech/doc). It is only meant as an introduction to group work and I will try to update it over time to reach a wider audience. As it is right now, it is mostly aimed towards computing students.

I am, by no means, an expert in the field. These notes reflect what I've learned, while reading up on DevOps, against my personal experience in group work. They also only take into account what may be relevant for students, rather than professionals.

The following topics are named after the slides in question, with the link to the slides at the bottom of the page.

## Background

Currently a 2nd year student in Computer Science with little to no experience in group work, apart from the odd summer project with friends, where no organisation was really needed. As such, decided to expand my knowledge and looked to industry standards to do so. These are my compiled notes on how to better structure your work as a team and how to operate at better efficiency.

## Student life

Typically, students have very well defined objectives and focus more on developing a product, rather than maintaining.
1. Deadline focused, meaning that the team knows exactly when to submit the project by, with little to no space for extensions.
2. Set of well defined criteria, which the program must hit to get full marks.
3. Different levels of knowledge within the group, with some students having a better graps on some topics than others.

## DevOps - Intro & Key Concept

DevOps is essentially Development and Operations combined. Development being the creation of new features or new products and operations being maintaining the existing product, with QA, InfoSec, IT Operations, making sure everything is running smoothly.

As such, DevOps ensures that there is complete transparency and collaboration between those two sides, thus making the product a combined effort without relying too much on handing over to the next person/team. It allows the team to treat everything as an experiment, due to relying on fast commits and continuous testing. Everything should be commmited to version control, including production and pre-production environments to make sure that, once change happens, it happens as close to a finalised state as possible. This in turn minimises downtime, minimises possible issues,  maximises the team's time.

## The Three Way

DevOps has three key components:
1. First Way - Flow: How to organise your team's work so everyone knows exactly what stage the product is in.
2. Second Way - Feedback: Dealing with issues that do occur. 
3. Third Way - Continual Learning and Experimentation: How to translate what happens during feedback to strategies the team will be able to use later on.

### Flow

#### 1. Kanban boards

Use of kanban boards allows every one in the group to know exactly which stage the product is in. A kanban board is organised into columns, labeled, as an example, from left to right, as "To do", "In progress", "To be tested" and "Done". An item is placed on the appropriate column, with the goal being to move all the items from the leftmost column to the rightmost column. Work is visible at all stages.

#### 2. Reduce WIP

People are generally bad at multitasking so avoid pilling up "In progress" items. A simple limitation of one item per "In progress" column ensures that your work is effectively better, as it deters you from trying to do too many things at once. Technical debt is a related term, defined by accumulating work, so your daily tasks focus on fixing previous items, rather than focusing on present issues.

#### 3. Limit batch size

Instead of doing a massive commit every week, opt to do daily, smaller commits. This ensures that any issues that might arise, are spotted quickly, instead of having to debug a sizeable portion of code. By doing this, it also keeps everyones code up-to-date, contributing to the overall transparency and collaboration between team members.

#### 4. Peer-review commits

Before each commit, have a team member test your code. You can do extensive testing and somehow miss a particular bug that will stop your product from working, and having someone re-test it, limits that chance. It also prevents the whole "It worked on my computer but not on a different computer".

#### 5. Use of feature-toggles

Further expanding on daily committing. Commit even if that particular function isn't quite ready. Have a toggle, such as a conditional, stopping that piece of code from running, but still keep a frequent commit cycle. Reiterates on previous points.

#### 6. Trunk based development

Avoid long running branches with your work in progress. Create fast lived branches and commit frequently. By doing so, you avoid merging conflicts and, any that do happen, are more easily fixed than if you were to have a long running on. Reiterates on previous points.

### Feedback

#### 1. See problems as they occur

Test frequently so you can spot any errors as soon as they happen. Avoid only testing after something has been committed.

#### 2. Swarm issues

The Andon cord system was used by Toyota where, if a fault was detected in the production line, the cord would be pulled and every worker would swarm to fix the problem. A similar approach is to be used as, if anything breaks your product, every one should stop everything that they are doing to fix the problem. By doing so, everyone learns what caused it, how to fix it should it happen again and how to mitigate its occurrance. Shared knowledge is key.

### Continual Learning and Experimentation

A single quote was used for this slide: 

```
"By removing blame, you remove fear; 
by removing fear, you enable honesty; 
and honesty enables prevention" 
-- Bethany Macri, Etsy
```

Avoid placing blame. Mistakes happen and no one should be heavily punished for them, as that creates the wrong kind of environment. Everyone should come together, learn from that mistake and carry on.

## Last tips

1. Wiki

Make a detailed written record of your progress. Most university related coursework requires some form of documentation and its easier if you do it as you go along, rather than writing everything once the product is finished. It also helps your team members know why you picked a particular way of doing things, letting them look at your code as a whole.

2. Agile/Scrum daily meetups

Have frequent meetups with your team members where you just update each other on your personal progress. A good framework is discussing: What you achieved during the previous days; What you hope to achieve the following days; What is limiting your ability to perform your planned work.

## Further Learning

Most of my research was based on the following books:

* ”The DevOps Handbook” -  Gene Kim, Jez Humble, Patrick Debois & John Willis – IT Rev Press
* “The Phoenix Project” - Gene Kim, George Spafford, and Kevin Behr

## Slides

[Speaker deck link to the slides](https://speakerdeck.com/stdlibdoh/devops-final)

## Conclusion

As mentioned, I will try to keep updatting these notes, to not only computing students. Any feedback or suggestions is greatly appreciated.

Twitter: @stdlibdoh
