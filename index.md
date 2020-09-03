## HW0: Introduction
Hi, my name is Joe Mezera. I am a senior here at the College of Charelston. I hit global in wingman. I like cars, and computers, and going to in person classes.


## HW1: Chapter 1
1.3: What are the four important attributes that all professional software should possess? Suggest four
other attributes that may sometimes be significant.
All software should be, dependable and secure, Efficient, Maintainable, and acceptable to the 
users(understandable, usable and compatible)
other attributes that may sometimes be significant are affordability, learnability, testability, portability.


1.8: Discuss whether professional software engineers should be licensed in the same way as doctors or
lawyers.

Although software engineers do not often directly hold their clients lives in their hands like doctors or lawyers may, there is still often times sensitive information being handled. A software engineer has the responsibility to protect any information that their software may receive from anyone it is not intended to reach. They also have a responsibility to not misuse their skills to gain access to things that were meant to be sealed. As with any job dealing with peoples personal details, it is the responsibility of the person handling the information to make sure that it remains safe and a license it a good way to ensure that the person handling the information is indeed qualified to do so. 


1.9: For each of the clauses in the ACM/IEEE Code of Ethics shown in Figure 1.4, propose an
appropriate example that illustrates that clause.

Public: Adding features that are requested by users
Client and employer: Creating functionalities requested by an employer that improve the environment for the client
product: Writing software that not only does what was requested, but is time and space efficient.
judgment: Refusing any work that they think is wronging or harmful to anyone. Refusing work that may be immoral. 
Management: Don't lie about experience or capabilities to potential clients, promote good morals within the software development team. 
profession: Advance yours and your teams skills by doing good work and promoting good software engineering practices. 
Colleagues: Promote healthy collaboration and make sure that the engineers are comfortable asking for help.
Self: Continuing to improve oneself from job to job and learning from those around you


1.10: To help counter terrorism, many countries are planning or have developed computer systems that
track large numbers of their citizens and their actions. Clearly, this has privacy implications. Discuss
the ethics of working on the development of this type of system.

It is hard to weigh the value of privacy for the citizens of a country against the potential value of their safety. Spying on, or tracking citizens clearly violates their privacy regardless of whether or not their privacy is supposedly protected by law. It is also hard to evaluate how much poeple knowing they're being watched changes their behavior, and therefore it is hard to know the extent that citizens are potentially being protected by this invasion of privacy. The ethics of working on a system meant to protect the public that also invades their privacy would have to be evaluated by the individual asked to do the project. There is no right or wrong answer, assuming the software is being used as intended, and therefore the engineer needs to weigh the pros and cons and decide whether or not it goes against their own personal beleifs. 

## HW2: Reflections on Software Engineering Practices

  In the articles, No Silver Bullet, Kode Vicious, and Google Code Repo there was one main commonality that they all addressed. Each article addressed the importance of sticking to good programming practices. The Silver Bullet article explored how, despite the many advancements programmers had made, none of them were the "Silver Bullet," that could solve the basic problems programmers had always faced. The Kode Vicious article is the author addressing the bad practices that expressed in the questions, and how they can be avoided in the future. The Google Code Repo article addresses they way google stores its code and the systems in place to make sure that all the code that gets pushed is acceptable, while also addressing the downsides of Googles solution of using a central repository for everything. 
  Something that every article addressed was the importance of doing everything correctly the first time. There is no substitute for good practices and neglecting them can cause problems down the line that there is no good solution for. In the first response in Kode Vicious the question is about whether or not they should continue to cherry pick code to match another branch or just push his current branch and address the issues it causes from there. The author never really answers the question but instead reminds them of the good coding practices that could have prevented the problem in the first place. The author pointed out that there was no good solution to his problem other than to learn from it. A similar organizational concern in the Google Code Repo arose when the idea of Google moving its code to a different version control system. Google has built a lot of infrastructure around its piper respository, a singular repository that houses all of googles code, and it would take a lot of effort to switch from a singular repository system like piper to a distributed version control system that utilizes, in Googles case, thousands of repositories. Although lots of thought has gone into building piper, if Google decides to switch to a DVCS, like the cherry picking guy, the longer he waits to do it, the more work that is going to have to be done to change it. 
    Another good practice that the articles address is the importance of keeping records of changes to software. Keeping records of changes in software can help prevent or fix future bugs in code, as well as informing other developers on the team what everything does, when code was updated, why it was updated, and the proces involved in creating the update. The Kode Vicious article pointed out that even if you think you can remember everything about your software, which you can't, your team doesn't neccessarily know everything you do and in order to function everyone needs to understand what is happening.
    All of the articles addressed the importance of good programming practices and the skills that come with them. Programmers need to stick to the way things work, documenting changes, keeping organized, and making sure everyone is on the same page. As it was addressed in the articles, there is no substitute for good programming practices and ther likely never will be.  
    
## HW3: Chapters 11 & 12

11.4 What is the common characteristic of all architectural styles that are geared to supporting software fault tolerance?
The software and hardware in a system are designed to be redundant and diverse

11.7 It has been suggested that the control software for a radiation therapy machine, used to treat patients with cancer, should be implemented using N-version programming. Comment on whether or not you think this is a good suggestion.
I don't think this is a good suggestion. A radiation therapy machine doesn't need to be available in high volumes and for a machine that performs sensative operations like radiation therapy there should be a human operator to catch an error. N-version programming would only increase costs on a likely already costly machine, as well as increasing risk by giving it the unnecessary ability to operate without a human operator. 

11.9 Explain why you should explicitly handle all exceptions in a system that is intended to have a high level of availability.
A system with a high level of availability is expected to be able to execute its operations whenever it is called upon to do so. If exceptions are not handled explicitly then the software could get stuck on the exception or shut down because it has a situation that it doesn't have instructions for how to deal with it. 

12.5 A train protection system automatically applies the brakes of a train if the speed limit for a segment of track is exceeded, or if the train enters a track segment that is currently signaled with a red light (i.e., the segment should not be entered). There are two critical-safety requirements for this train protection system:
 The train shall not enter a segment of track that is signaled with a red light. 
 The train shall not exceed the specified speed limit for a section of track.
Assuming that the signal status and the speed limit for the track segment are transmitted to on-board software on the train before it enters the track segment, propose five possible functional system requirements for the onboard software that may be generated from the system safety requirements.
1. The system should regularly check the current speed of the train
2. The system should apply the brakes if the train is exceding the speed limit on the current section of track
3. The system should regularly check the track status of the current segment of track
4. The system should apply the brakes if the current track segment is signaling a red light
5. The system should regularly check the signal status of the upcoming track segment
