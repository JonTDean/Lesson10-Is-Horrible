# To Whomever is Reading this

<Details> <Summary>Read this if you're from Woz-U</Summary>
	<p>Fix this lesson for all that is holy</p>
	<ins>Reasons Why</ins>:
	<ol>
		<li> Everytime I read this lesson I question my existence. </li>
		<li>It's just bad bro. The person who wrote this genuinely didn't care about the lessons. Almost as if you stole this from the internet, hmmmm.</li>
		<li>I've taught third graders that have better writing skills than the creator of this lesson and I.</li>
	</ol>
</Details>

For my thoughts on the horrible original design here is the <a href="https://github.com/JonTDean/Lesson10-Is-Horrible/blob/main/OriginalCriticism.md">Text for that</a>

<h1>Lesson 10 Final Project</h1>

<h2> Revised - AN ACTUAL SOFTWARE DESIGN SHEET </h2>

<div className="Part_One">
	<h3><ins>Part 1 : Undoing the Abysmal Mess</ins></h3>
	<br/>
	<ol>
		<li> 
		<p>Create a Program Named <code>FinalProject</code>. Rename the File to <code>ContractorPayrollDemo</code>. Rename the Class <code>FinalProject</code> to <code>ContractorPayrollDemo</code></p>
			<Details> 
				<Summary> Image describing what is being asked. </Summary>
					<img src="https://i.imgur.com/EyaFG7m.png" />
			<Details> 
		</li>
		<br/>
		<br/>
		<li> Inside of <code>ContractorPayrollDemo/Program.cs</code> Create a Class called <code>Employee</code>.
			<br/>
			<Details> 
				<Summary>Fields and Types of <b>Class</b> <b><i>Employee</i></b> </Summary>
				<ul>
					<br />
					<li> A Public Field with a Type of <code>String</code> named <code>employeeIdentificationNumber</code>. Give this a Getter/Setter. </li>
					<br />
					<li> A Public Field with a Type of <code>Byte</code> named <code>numberOfHoursWorked</code>. Give this a Getter/Setter. </li>
					<br />
					<li> A Public Field with a Type of <code>Double</code> named <code>ratePerHour</code>. Give this a Getter/Setter. </li>
					<br />
					<li> A Public Field with a Type of <code>String</code> named <code>stateName</code>. Give this a Getter/Setter. </li>
					<br />
					<li> A Public Field with a Type of <code>Double</code> named <code>payCheck</code>. Set the value at instantiation, using the product of <code>ratePerHour</code> and the <code>numberOfHoursWorked</code>. </li>
					<br />
					<li> A Public Read Only Field with a Type of <code>Float</code> named <code>currentTaxRate</code>. Set the value at instantiation, using the <code>stateName</code> to refer to the API from Taxee. </li>
					<br />
					<li> A Public Type of <code>Double</code> named <code>taxAmountTotal</code>. Set the value at instantiation, use the product of <code>payCheck</code> and <code>currentTaxRate</code>. </li>
					<br />
				</ul>
			</Details>
		</li>
		<br/>
		<li> 
			<p>In the development field, recreating something that exists is bad practice and only horrible developers would even suggest doing that. Because we are amazing developers (and not savages) let's use an API and connect to it: <a href="https://taxee.io/dashboard">Taxee API service</a>.</p>
		</li>
		<br/>
		<li>
			<p>Now since this is a Web Development class, learning how to fetch an API should be one of the first things we learn after the basics. If you want to read up on how to retreive data from an exposed API <a href="https://docs.microsoft.com/en-us/aspnet/web-api/overview/advanced/calling-a-web-api-from-a-net-client">go here for fetch in .net</a>. Learning to read the documentation is necessary as a developer skill.</p>
		</li>
		<br/>
		<li>
			</p>Let's look at The User Story (flow of the programs actions, when someone is using the Application) </p>
			<Details> 
				<Summary>The User Story should perform like this.</Summary>
				<ol>
					<br />
					<li> Start Application </li>
					<br />
					<li> Ask the user to Create an Employee and to fill out the Requested Information. The user should be able to do this as many times as they want to. </li>
					<br />
					<li> Allow the user to pick which Employee to display. </li> 
						<ul> 
							<li>We can do the Employee Display with a technique called Pagination using the <a href="https://docs.microsoft.com/en-us/dotnet/framework/data/adonet/sql/linq/return-or-skip-elements-in-a-sequence?redirectedfrom=MSDN">.Skip() and .Take()</a> Methods </li>
						</ul>
					<br />
					<li> Display the Employee Information when the User gives a Selection. </li>
					<br />
				</ol>
		</li>
</div>
<hr />
<div className="Part_Two">
	<h3><ins>Part 2 : Undoing the Abysmal Mess Electric Boogaloo</ins></h3>
	<ol>
		<br />
		<li>Let's create a new file inside of our project by clicking <code>add -> New File -> .net CLI</code> and let's name it <code>ContractorPayrollDemoSort</code>.</li>
		<br />
		<br />
		<li>Let's create a <code>class</code> called <code>Sort</code></li>
		<br />
		<br />
		<li>Add the ability to sort the Employees by the following criteria:
			<Details> 
				<Summary>Methods of <b>Class</b> <b><i>Sort</i></b> </Summary>
				<ul>
					<li> Name, returns a sorted collection of the employees by alphabetical order. </li>
					<br />
					<li> Total Amount Paid, returns a sorted collection of the employees by Highest Total Amount Paid To Lowest Total Amount Paid </li>
					<br />
					<li> Total Hours worked, returns a sorted collection of the employees by Highest Total Hours Worked to Lowest Total Hours Worked </li>
					<br />
					<li> Total State Tax Paid, returns a sorted collection of the Employees by Highest Tax Paid to Lowest Tax Paid </li>
				</ul>
			</Details>
		</li>
		<br />
		<li>
			<p>Inside of <code>ContractorPayrollDemo/Program.cs</code> let's add a using statement to the top of the file.</p>
			<code>using ContractorPayrollDemoSort;</code>
		</li>
		<br />
		<br />
		<li>Lets add functionality so the user can pick which sort he wants to use. Let's also give the option to remove the sort.</li>
		<br />
		<br />
</div>
	
<h3><ins>EXTRA CREDIT</ins></h3>
<p>Add functionality to reverse all of the sort methods.</p>

