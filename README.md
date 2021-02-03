# Lesson10 Is Horrible

Fix this lesson please. 

<ins>Reasons Why</ins>:

1. Everytime I read this lesson I question my existence.

2. It's just bad bro. The person who wrote this genuinely didn't care about the lessons. Almost as if you stole this from the internet, hmmmm.

`Disclaimer`: Any text that looks like `this` is a comment from myself.

-------

## Lesson 10 Final Project


### Original

#### Directions

`Now concerning the "Directions", this can get eliminated completely, it has absolutely nothing to do with the topic at hand. It's quite literally just over-exposition, like this comment.`

Welcome to the Final Project for the Core C# course! Great job making it this far! This Final Project will be different from the Hands-On projects you have previously seen in a couple of different ways. For the Final Project, you will be putting together the numerous topics you have learned into one large project. It is designed to mimic real problems which you may face in your career, so it may be a challenge for you and will also take several hours. Take this project step-by-step and be aware that the project description below is written to be a bit less specific than previous Hands-Ons. The Final Project is supposed to challenge you to do some problem solving to figure out how to accomplish a task. You can always review past lessons or use a Google search if needed. Good luck!
Setup

`So Create a C# Project named FinalProject Or Create a C# Project Named Contractor Payroll??????`
Create a new C# project as you have done throughout this course. Name this project finalProject.

#### Part 1

` This is the most unorganized mess I've ever read. How does the author exepct for us to simulate a real world environment if we cannot talk to our client? We are Software Developers not mindreaders. In a real world environment there is a back and forth in order to clarify responsibilities. This is written by someone who has never worked in a professional environment, least of all a Software Development field.`

`Where does the person asking us want this? Preference is definitely used here, however in an environment where you are being "professional"
 following a ruleset in order to have your code be readable is necessary.`

Create a program named ContractorPayrollDemo that declares an array of 10 Employee objects.

` What is this? Did the writer think of this over the course of 10 seconds? Why are we declaring something prior to specifying the Blueprint for what we want to display? Horrible Software Development writing here. Why are we spamming the user with 300 lines of text? That is not user friendly. Let's have some tact.`

Prompt the user for data for each object and display 10 objects.

`Data fields ok. What types are we using, does the author want us to use an int16 for the employee Identification number? Are we simulating a real EIN and using a string format? What Data Types are we using for the rest. This is supposed to simulate a professional environment so where are our strict instructions?`

Data fields for Employee objects include an employee identification number, number of hours worked, rate per hour, and state where work was done. 

`Worst offender of all. Why is this text Classifying the first two, this needs to be specific not so general; specification of what needs to happen is necessary. What tax??????? When did tax come about in this entire Fake Software Design Sheet prior to this sentence? I still have no idea what is asked here, horrid practice. Just saw there's another variable named Paycheck amount, why is this written like this? This is simulated to be hard when it's just written by someone with the writing skills of a kindergartner.`

Include a property with get and set accessors for the first two data fields, but make the tax a read-only property. The state tax should be calculated whenever the amount of the paycheck is set.

`Does the author understand the complexity of this? The author is asking for us to calculate taxes without using the appropriate amount of information. We need to add to this data, the above is incomplete and is one of the worst assignments I've ever had the displeasure of reading in my entire life. Fire the author, they scammed Woz-U.`

Note: You will need to use a state tax calculator to calculate the appropriate state tax. Remember some states may not have a state tax, some have a progressive system, and others have a flat tax.


#### Part 2

`Is this really a part? This is sad attempt at trying to implement the algorithm section. This is just sad and lackluster. Fire your curriculum writer they genuinely suck at their job and do not care about the content they put out.`

Create a program named ContractorPayrollDemo2 so that after the initial 10 Employee objects are displayed and they are sorted in order by the amount of their paycheck and total state tax, they are then displayed again.

----------

### Revised

#### Part 1 : Abysmal Mess

1. Create a Program Named *FinalProject*. Rename the File to *ContractorPayrollDemo*. Rename the Class *FinalProject* to *ContractorPayrollDemo*

	<img src="https://i.imgur.com/EyaFG7m.png" />

2. Inside of `ContractorPayrollDemo/Program.cs` Create a Class called Employee.
	* Employee Should have the following properties/fields
  
		* A Field with a Type of **String** named **employeeIdentificationNumber**. Give this a Getter/Setter.

		* A Field with a Type of **Byte** named **numberOfHoursWorked**. Give this a Getter/Setter.

		* A Field with a Type of **Double** named **ratePerHour**. Give this a Getter/Setter.
		
		* A Field with a Type of **String** named **stateName**. Give this a Getter/Setter.
		
		* A Field with a Type of **Double** named **payCheck**. This is set when the **ratePerHour** and the **numberOfHoursWorked** is set.

		* A Read Only Field with a Type of **Float** named **currentTaxRate**. This is set when the **stateName** is set.
		
		* A Read Only Field with a Type of **Float** named **taxAmountTotal**. This is set when the **payCheck** and **currentTaxRate** is set.

3. In the development field, recreating something that exists is bad practice and only horrible developers would even suggest doing that. Because we are amazing developers (and not savages developing on the *Commodore 64*) let's use this site and connect to it's [API service](https://taxee.io/dashboard).

4. Now since this is a Web Development class, learning how to fetch an API should be one of the first things we learn after the basics. If you want to read up on how to retreive data from an exposed API [go here for fetch in .net](https://docs.microsoft.com/en-us/aspnet/web-api/overview/advanced/calling-a-web-api-from-a-net-client). Learning to read the documentation is necessary as a developer skill.

5. The User Story (flow of the programs actions, when someone is using the Application) should perform like this.

	1. Start Application

	2. Ask the user to Create an Employee 10 times and to fill out the Requested Information.

	3. Allow the user to pick which Employee to display.

		* We can do the Employee Display with a technique called Pagination using the [.Skip() and .Take()](https://docs.microsoft.com/en-us/dotnet/framework/data/adonet/sql/linq/return-or-skip-elements-in-a-sequence?redirectedfrom=MSDN) 

	4. Display the Employee Information when the User gives a Selection.
	
#### Part 2

6. Add the ability to sort the Employees by the following criteria:
	
	* Name
	* Total Amount Paid
	* Total Hours worked
	* Total State Tax Paid


