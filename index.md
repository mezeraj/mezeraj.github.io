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
2. The system should apply the brakes if the train is exceding the speed limit of a section of track it is nearing
3. The system should apply the brakes if the upcoming track segment is signaling a red light
4. The system should apply the brakes if the current track segment is signaling a red light
5. The system should regularly check the signal status of the upcoming track segment

## HW4: Relections on Software Failures

  After reading the articles from the past two weeks the common theme between the readings is software failure do to neglegence. In each of the articles addressing software failures on major projects the blame is placed on inadequacies in the software development process. In many of the projects it is specifically put on an inadequate or rushed testing phase or on an inadequate procedure that lead the programmers to misinterpret their instructions. These failures are great examples, and unfortunate learning experiences, that show the importance of the software development process and having good software engineering practices. Although none of my projects have caused the failure of a multi million dollar project or cost someone their life, I know that there are many times I could have avoided problems if I had been more organized and thorough in my process. 
    
   The multiple failures discussed in the Spacecraft Accidents article are examples of poor communication between software engineers and people working on the spacecraft, issues that could have been spotted with more extensive testing or by providing more precise instructions to the programmers to give them a better understanding of their job. One of the examples of miscommunication is in the Mars Climate Orbiter where everything was done right except one part of the code was done in American units instead of metric, causeing the probe to overshoot into the atmosphere and crash land on Mars. This could have been caught with better testing or with more explicit instructions. The Mars Polar Landers failure was likely caused by a miscommunication as well. The designers of the lander had an understanding that there was a false positive for detecting the ground when the legs are deployed and it was to be ignored. The software engineers didn't know about this so when the MPL deployed its landing gear it fell to the surface and was destroyed. 
   
   The FBI went millions of dollars over budget and years over the deadline trying to create a central database for all of their divisions. The original project cost $170 million and when it was delivered it was riddled with bugs and unusable. This caused the FBI to bandaid the project so that they had a usable system until their Sentenal project was done. The sentenal project ran over budget and over its deadline multiple times because it wasn't up to par with the FBIs needs time and time again. The developers of the project were also lazy with their progress reports which lead to misinformation about where they were in the process. When the Sentinal project was announced as finished in 2012 but then in 2014 the FBI made another statement that the project was still not in total shape. The initial failures of the sentinal project caused a snowball effect that laneded the project years late and millions over budget. 
    
   These failures in software engineering highlight the importance of communication in the software development process. Miscommunication or misleading members of a team, a client, or an employer can lead to heavy financial consequences like in the spacecraft accidents and the FBI database, or even crippling or killing someone like in the case of the Therac-25 accidents. It is important to treat the software development process like any other engineering process. It seems like the government in the early 2000's tended to overlook the importance and the impact that bad code could have on a project. Good software practices shouldn't be optional especially in high risk scenarios.
   
## HW5: Chapter 4 and reflections

4.5) Using the technique suggested here, where natural language descriptions are presented in a standard format, write plausible user requirements for the following functions:
  
  An unattended gas pump system that includes a credit card reader. The customer swipes the card through the reader, then specifies the amount of fuel required. The fuel is delivered and the customer's account debited.
  The system should prompt the user to enter a pin before charging the card
  
  The system should require the user to specify a fuel grade before allowing the user to pump gas
  
  The system should require the rate at which the fuel is pumped by the user via a trigger or button
  
  The system should credit the customers account if they finish fueling before all the fuel they paid for is pumped. 
  
  The system should stop pumping fuel if it detects that the vehicle is full.
  
  The cash-dispensing function in a bank ATM.
  
  The system should verify the card being used is valid
  
  The system should prompt the user to enter a pin and verify the validity of the pin
  
  The system should ask the user how much money they would like do be dispensed
  
  The system should check that the user has sufficient funds in their account to withdraw cash
  
  The system should dispense the correct amount of cash to the user
  
  In an internet banking system, a facility that allows customers to transfer funds from one account held with the bank to another account with the same bank.
  
  The user should have to confirm that they are an authorized owner of the account via a passowrd or pin
  
  The user should specify which acocunt(s) they want to transfer funds to and from
  
  The system should verify that both accounts are indeed with that bank
  
  The user should confirm that this action is indeed they one they want to do
  
  The funds should be available in the other account instantaneously
  
4.6) Suggest how an engineer responsible for drawing up a system requirements specification might keep track of the relationships between functional and non-functional requirements.
The list of requirements could be organized by a list of non-functional requirements with a list under each non-functional requirements of functional requirements that would help the non-functional requirements meet their objectives. For instance, If a non-functional requirement is that at any given time the nuclear plant can be shut down within five minutes, functional requirements could be that the system should generate a warning to shut down if it gets too hot, the system should shut down if (combination of actions) is completed, the system should monitor the temerature and provide live updates.

4.7) Using your knowledge of how an ATM is used, develop a set of use cases that could serve as a basis for understanding the requirements for an ATM system.

Depositing money allows the user to add money to their account by putting physical bills in the ATM. The user first must enter their card and pin to prove they are a verified user of the account. The user then selects the enters the amount of money they are depositing. The user then puts the money in the machine and the machine verifies that they amount of money the user put in the machine matches the amount they said they were depositing. If the amounts matches then the machine informs the user that they have successfully added money to their account, provides them with a receipt, and returns their card to them.

Withdrawing money from the machine allows the user to withdraw money from their account in the form of physical bills. The user must enter their card and fin to prove that they are a verified user of the account. The user then selects the amount of money they would like to withdraw. The machine checks to see if the user has enough money in their account to withdraw the desired amount and then the machine checks to make sure it has enough money to provide the user the desired amount. If both cases are true then the machine supplies the user with their money, prints a receipt, and ejects their card. 

chapter 4 readings)

The theme of this weeks readings was understanding the requirements of code before beginning to write it. It is important to understand exactly a program needs to be able to do and how well it needs to be able to do each thing in order to write it. Which functionalities need to be secure, which ones need to be fast and what things might not need to be done at all that could have slowed down development. Using a test first development system as discussed in the article can help the engineers understand the functional and non-functional requirements of a system. By developing a test for the code before the code itself there is a set of minimum standards that the code needs to meet, so long as the testing is thorough.

## HW6: Chapter 2

2.1) Suggest the most appropriate generic software process model that might be used as a basis for managing the development o fhte following systems. Explain your answer according the the type of system being developed:

A system to control antilock braking in a car: In an antilock brakeing system safety is of the utmost importance so a waterfall model would be the most appropriate. The system should be thouroughly thought through and tested before it is implemented into a system.

A virtual reality system to support software maintinence: Incremental development would be most appropriate in this scenario. Features and processes could be released as the work to continue to add functionality to the VR system and it can be tested on the system without danger. 

A university accounting system that replaces an existing system: for this solution incremental development could be used so that the new software could be used and improved upon as it is being developed and the old software can still be used until the new is ready. This way the new software is rolled out more smoothly as it isnt implemented all at once. 

An interactive travel planning system that helps users plan journeys with the lowest environmental impact: Incremental development would be best for this system. The system could be launched with base features, and with no risk to any users, could be improved upon with added features along the way. 

## HW7: Chapter 5 and 6

[Exercise 5.3](https://drive.google.com/file/d/1XmLOSJYy4pYkaqUT9gtgomHJCgv__hgI/view?usp=sharing)

[Exercise 5.5](https://drive.google.com/file/d/1RkNDeLBhRQeBuTr_PQI2jD36ekQiukMP/view?usp=sharing)

[Exercise 5.7](https://drive.google.com/file/d/1lnpXrv8e1Uv579vmU9pezC0GHprqrHJb/view?usp=sharing)

[Exercise 5.8](https://drive.google.com/file/d/1wspXiD5MXAMwdwI8SfrI2pdowVQtba8S/view?usp=sharing)
It is important to develop both activity and sequence diagrams so that you can observer the physical processes associated with a system as well as the digital processes. 

[Exercise 6.4 Ticketing System](https://drive.google.com/file/d/1anflByEZXrQqy6bwH7SARCYcJn3eN3KH/view?usp=sharing)

[Exercise 6.4 Video Conference](https://drive.google.com/file/d/1wQt-3Wq12Otfb4dGf9tNqEE6XfVd7Bf1/view?usp=sharing)

[Exercise 6.4 Robot Vaccum](https://drive.google.com/file/d/1sFSgT6CYfJ3HTq6X5bvmaas1qdf6kAcY/view?usp=sharing)

## HW8: Mythical Man Month

  Mythical Man Month discusses the pros and cons, mostly cons, of having a large software team to develep software simultaneously. Since software development often can not be divided up into evenly distributed bits of code, teams must work together to solve problems linearly, with one lead mind guiding the process so that eveything stays consistent. This does not mean that there cannot be large teams for large projects though. There are certain projects that require a lot of people to work on them or they would take too long. This just means that on a large projects there needs to be a small number of drivers with a large support team behind them. The drivers need to focus on driving while the other members of the team help by doing their own tasks. 
  Mythical Man Month also discusses that most team leads like have a small team of sharp people rather than an army of people to command. This is heavily reflected in the softwrae engineering process today and in the surgical team example from the text. There only needs a be a small amount of people writing the code for a project since many projects need to be done linearly. However, they also need ideas from others, someone suggesting ideas or researching better or more efficient ways to do things. This is like a larger scale version of paired programming from our CS labs. There is one person writing and one person simply presenting ideas to the person writing. This way everyone is familiar with the code being written and there can be multiple minds figuring out the process. The actual typing part of coding isn't what takes a long time, its the problem solving things along the way. The texts discusses how its hard to have a timeline for programming projects becasue they can only predict how long it will take if there are no problems, and it is very difficult to predict what kinds of problems may be encountered along the way or how long it will take to solve them. 
    The entire idea of the Mythical Man Month is that man power does not equal time in programming. Each project cannot act as a multi threaded project where each member gets its own task. Each team must function as one cpu where they all work together so solve the current problem they are working on by each member completing their own task. This is the analogy that kept coming to mind while reading the text, which I think fits the subject well. While many workloads can be accelerated with more man power, some of them benefit most from having one efficient driver running the whole show. 


## HW9: Chapter 8 and refelections on testing

8.7: Someone requests data from the weather station system but it has been damaged by the environment and not all of the gagues are working. Since the satelite uplink bandwidth is low and the connection is slow, it cannot send all of the data at once. 

8.10: The problem with testing until the budget runs out is that if the budget runs out before testing is completed then the software may still have significant bugs remaining. If there is more than enough budget to run tests after testing is complete then that is a good thing but, if there isn't enough money to do the testing the company risks releasing a faulty product which, if the product has sensitive information or does tasks that are high risk, creates lots of potential risk for using the software in the real world. 

Reading Relection: One of the major takaways from the readings was the extensive planning that goes into testing as well as the different processes associated with different types of testing. Well planned and organized tests can lead to better and more useful test cases as well as leaving more time and money to test other processes. It is also important that the people testing the product understand the full intentions and uses of the product. The testers can run every method and check for outcomes but if they don't understand the uses of the software then it can be harder to understand where and why bugs are being produced, or why the outcomes are what they are. 


## HW10: Chapter 15

15.10: Many of the issues brought up in the question are solved in the contract between the company paying for the software and the company writing the software. If it is specified that the company paying for the software owns all of the code software then they can go about and change and reuse the code, hiring whoever they want to do so. However, if the company writing the code owns it then the copmany paying for it could be somewhat obligated to go back to them for changes. Which also makes the most sense since they likely understand it better anyway. If they do go to someone else then the original software writing company might feel obligated to reimbursement for others using their code, especially if it is used to create new systems,

## HW11: Chapter 9

9.8: Fault repairs to fix bugs and vulnerabilites. This type of maintinence is used to fix issues that should not have existed in the first place. Bug fixes, design errors and requirements errors. These can be lessened through thourough testing, but they are almost impossible to eliminate. 

Environmental adaptation to adapt the sofware to new platforms and environments. This type of maintenance is requred when parts of a system are no longer supported.  If an operating system goes out of use, or hardware becomes too old to maintain. Environmental changes can require moving large amounts of a system from one platform to another.

Functionality addition to add new features and support new requirements. This maintinence is required when the needs of the business change. It could be new tools, features, or layouts to a system. These will happen regularly but they usually do not require a massive rewrite. 

It can be difficult to distinguish between different types of maintinence because one type of maintinence may lead to another. For instance if a company wants to add new features that aren't supported by their current system, there may be environmental adaption required as well, and any type of maintinence can lead to repairs, even repairs can lead to more repairs. 

9.10: Engineers have a professional responsibility to create code that can be easily maintained. They should create code so that someone comeing in having never seen it before can understand it without completely stripping it down. Engineers should write code how the same way they would like code to be written for them. Employers not having specific requirements for code maintinence standards should be understood as them assuming you know how to best write the code and that way you can be a more efficient worker. 

## HW12: Chapter 16

[Exercise 16.9 part 1](https://drive.google.com/file/d/1pwGcnbICT27Kfd21PtDLDNP-6cTfTWfS/view?usp=sharing)

[Exercise 16.9 part 2](https://drive.google.com/file/d/13ibvZKje3GlvpCNVcQ17X2Z1LzoBHagt/view?usp=sharing)

## HW13: Chapter 17
Accessability: The availability of the service will no longer be based on whether or not the computer in front of a user is working, it will be based on both the users machine and the serverside machine functioning. On top of that if the service fails on the server side then the service fails for all users and not just on one computer. This risk can be reduced by having back ups on the server side to make sure that if one thing fails that everything doesn't fail. Redundancy. 

Latency Issues: A service based on the users computer will always be more responsive than a service based in the cloud and running on a users computer. If actions need to be completed quickly and accurately then latency can become an issue even if it is less than a second. This can be resolved with fast user internet and fast servers from the provider. 

Financial: A service bought by a user and installed on a computer usually has a single, larger, up front cost, while a service provided over the internet and hosted somewhere will usually be paid for in monthly plans. If for some reason the company cannont pay for the service then they could lose all of that data that was stored on the server side. This can be resolved by backing up data in house.
