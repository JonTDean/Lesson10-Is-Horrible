## Lesson 10 Final Project Original

### Directions

`Now concerning the "Directions", this can get eliminated completely, it has absolutely nothing to do with the topic at hand. It's quite literally just over-exposition, like this comment.`

Welcome to the Final Project for the Core C# course! Great job making it this far! This Final Project will be different from the Hands-On projects you have previously seen in a couple of different ways. For the Final Project, you will be putting together the numerous topics you have learned into one large project. It is designed to mimic real problems which you may face in your career, so it may be a challenge for you and will also take several hours. Take this project step-by-step and be aware that the project description below is written to be a bit less specific than previous Hands-Ons. The Final Project is supposed to challenge you to do some problem solving to figure out how to accomplish a task. You can always review past lessons or use a Google search if needed. Good luck!
Setup

`So Create a C# Project Named: "Final Project" Or Create a C# Project Named: "Contractor Payroll"??????`

Create a new C# project as you have done throughout this course. Name this project finalProject.

### Part 1

` This is the most unorganized mess I've ever read. How does the author expect for us to simulate a real world environment if we cannot talk to our client? We're Software Developers not mindreaders. In a real world environment there is a back and forth in order to clarify responsibilities. This is written by someone who has never worked in a professional environment, least of all a Software Development field.`

`Where does the person asking us want this? Preference is definitely used here, however in an environment where you are being "professional" following a ruleset in order to have your code be readable is necessary. ESPECIALLY if you have 30 different people writing it. Template programming exists for a reason: https://en.wikipedia.org/wiki/Template_metaprogramming << This increases readability.`

Create a program named ContractorPayrollDemo that declares an array of 10 Employee objects.

` What is this? It took the writer 30 seconds to write this god awful lesson. Why are we declaring something prior to specifying the Blueprint for what we want to display? Horrible Software Development writing here. Why are we spamming the user with 300 lines of text? That is not user friendly. Let's have some tact.`

Prompt the user for data for each object and display 10 objects.

`Data fields ok. What types are we using, does the author want us to use an int16 for the employee Identification number? Are we simulating a real EIN and using a string format? What Data Types are we using for the rest. This is supposed to simulate a professional environment so where are our strict instructions?`

Data fields for Employee objects include an employee identification number, number of hours worked, rate per hour, and state where work was done. 

`Worst offender of all. Why is this text Classifying the first two, this needs to be specific not so general; specification of what needs to happen is necessary. What tax??????? When did tax come about in this entire Fake Software Design Sheet prior to this sentence? I still have no idea what is asked here, horrid practice. Just saw there's another variable named Paycheck amount, why is this written like this? This is simulated to be hard when it's just written by someone with the writing skills of a slug.`

Include a property with get and set accessors for the first two data fields, but make the tax a read-only property. The state tax should be calculated whenever the amount of the paycheck is set.

`Does the author understand the complexity of this? The author is asking for us to calculate taxes without using the appropriate amount of information. We need to add to this data, the above is incomplete and is one of the worst assignments I've ever had the displeasure of reading in my entire life. Fire the author, they scammed Woz-U.`

Note: You will need to use a state tax calculator to calculate the appropriate state tax. Remember some states may not have a state tax, some have a progressive system, and others have a flat tax.


### Part 2

`Is this really a part? This is sad attempt at trying to implement the algorithm section. This is just sad and lackluster. Fire your curriculum writer they do not care about the content they put out.`

Create a program named ContractorPayrollDemo2 so that after the initial 10 Employee objects are displayed and they are sorted in order by the amount of their paycheck and total state tax, they are then displayed again.
