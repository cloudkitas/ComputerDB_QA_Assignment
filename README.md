# ComputerDB_QA_Assignment
A project for Backbase QA Role 


READ ME 

Design Choices:
-	Manual test scripts were written in Gherkin. This was opted due to the time available to prepare the regression bucket, the easiness to write Gherkin-like scripts and the value they provide in helping the majority the stakeholders to understand the purpose of a specific test. 
o	This regression test suite has  a limitation in the sense that I could have also written the automation tests to follow the BDD Gherkin approach. By writing automation Scenarios and feature Files that would execute the manual scripts. However due to configuration issues I made the decision to use instead a Page Object Model Framework for the automation suite. 
-	Automation Suite – Java Based using Selenium WebDriver.
o	Follows a page object model framework supported by the TestNG framework for the execution runs and reporting of the automation test cases. 
o	Packages include:

Automation Suite Structure

Page Object Model Framework
Computers Main Page
The computers main page - displays the list of records on the database, initiating point for creating new and opening existing records 
Computers Record Page 
The page for a specific existing computer record – displays computer details and is the initiating point for Deleting and Editing the record.
Add a Computer Page
Buttons: Create This computer; Cancel


Choice of Regression Tests:  
Please refer to the excel file attached in the project folder for a detailed explanation of why a specific test has been included in the regression 
The regression bucket aims to test the functionality across the following functional areas, which have been chosen due to the reasons that follow.
-	Screen UI Validations 
o	Tests to validate if the UI remains as expected – From an aesthetics perspective if it contains all the elements users expect to be present on the screen. These tests are spread across the 3 key pages: 
o	Elements validated include:
	Web App main title page
	Buttons are visible on the page
	Input fields are visible on the page
	Table contain the expected columns
-	Buttons Functionality 
o	Tests to validate the buttons functionality on each page 
	Computers Main Page
•	Buttons: Add, Next, Previous 
	Computers Record Page 
•	Buttons: Delete this computer; Save this Computer; Cancel
	Add a Computer Page
•	Buttons: Create This computer; Cancel

-	CRUD Functionality
o	Test to validate records can be created 
o	Records can be updated 
o	Records can be deleted
o	Records can be retrieve from the DB 

-	Fields Validations 
o	Tests to validate the field validation for those fields which have validations including: Computer Name, Introduced date, Discontinued date
o	These tests include: Boundary analysis (invalid dates), incorrect format and a decision table to ensure all possible combinations valid/invalid combinations across the 3 fields.  
-	


Implementation Guidelines:
-	Set WebDriver device specific properties 
o	On TestBase Change the location of webdriver to match your own specific environment 

