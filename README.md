# Lesson10 Is Horrible

Fix this lesson please. 

<ins>Reasons Why</ins>:

1. Everytime I read this lesson I question my existence.

2. It's just bad bro. The person who wrote this genuinely didn't care about the lessons. Almost as if you stole this from the internet, hmmmm.

-------

For my thoughts on the horrible Original design here is the [Text for that](https://github.com/JonTDean/Lesson10-Is-Horrible/blob/main/OriginalCriticism.md)

----------

## Lesson 10 Final Project


### Revised - AN ACTUAL SOFTWARE DESIGN SHEET

#### Part 1 : Abysmal Mess

1. Create a Program Named *FinalProject*. Rename the File to *ContractorPayrollDemo*. Rename the Class *FinalProject* to *ContractorPayrollDemo*

	<img src="https://i.imgur.com/EyaFG7m.png" />

2. Inside of `ContractorPayrollDemo/Program.cs` Create a Class called Employee.
	* Employee Should have the following properties/fields
  
		* A Field with a Type of `String` named `employeeIdentificationNumber`. Give this a Getter/Setter.

		* A Field with a Type of `Byte` named `numberOfHoursWorked`. Give this a Getter/Setter.
		
		* A Field with a Type of `Double` named `ratePerHour`. Give this a Getter/Setter.
		
		* A Field with a Type of `String` named `stateName`. Give this a Getter/Setter.
		
		* A Field with a Type of `Double` named `payCheck`. Set the value in the default constructor, using the `ratePerHour` and the `numberOfHoursWorked` as reference.

		* A Read Only Field with a Type of `Float` named `currentTaxRate`. Set the value in the default constructor, using the `stateName` as reference.
		
		* A Read Only Field with a Type of `Float` named `taxAmountTotal`. Set the value in the default constructor, using the `payCheck` and `currentTaxRate` as reference.


3. In the development field, recreating something that exists is bad practice and only horrible developers would even suggest doing that. Because we are amazing developers (and not savages developing on a *Commodore 64*) let's use this site and connect to it's [API service](https://taxee.io/dashboard).

4. Now since this is a Web Development class, learning how to fetch an API should be one of the first things we learn after the basics. If you want to read up on how to retreive data from an exposed API [go here for fetch in .net](https://docs.microsoft.com/en-us/aspnet/web-api/overview/advanced/calling-a-web-api-from-a-net-client). Learning to read the documentation is necessary as a developer skill.

5. The User Story (flow of the programs actions, when someone is using the Application) should perform like this.

	1. Start Application

	2. Ask the user to Create an Employee 10 times and to fill out the Requested Information.

	3. Allow the user to pick which Employee to display.

		* We can do the Employee Display with a technique called Pagination using the [.Skip() and .Take()](https://docs.microsoft.com/en-us/dotnet/framework/data/adonet/sql/linq/return-or-skip-elements-in-a-sequence?redirectedfrom=MSDN) 

	4. Display the Employee Information when the User gives a Selection.
	
#### Part 2

6. Let's create a new file inside of our project by clicking `add -> New File -> .net CLI` and let's name it *ContractorPayrollDemoSort*.

7. Let's create a class called *Sort* 

8. Add the ability to sort the Employees by the following criteria:
	
	* Name, sort the employees by alphabetical order.

	* Total Amount Paid, sort the employees by Highest Total Amount Paid To Lowest Total Amount Paid 

	* Total Hours worked, sort the employees by Highest Total Hours Worked to Lowest Total Hours Worked
		
	* Total State Tax Paid, sort the Employees by Highest Tax Paid to Lowest Tax Paid
	

9. Inside of `ContractorPayrollDemo/Program.cs` let's add a using statement to the top of the file. 

	```csharp

	using ContractorPayrollDemoSort;

	```	

10. Lets add functionality so the user can pick which sort he wants to use. Let's also give the option to remove the sort.

EXTRA CREDIT:

11. Add functionality to reverse all of the sort methods.

