# Web-rostering-App
Unity software project
3          Requirements	
USE CASE DIAGRAM
 

 
FUNCTIONAL REQUIREMENTS SPECIFICATION
 Admin functional requirements
F.1 Employee details

Req.ID	Description	Priority
 F1.1	 View employee details	 High
 F1.1.1	  When the admin logs in and clicks the employee list button, the application will list all the current employees on the webpage.
 F1.1.2	 When the admin clicks the key icon, the application allows the admin to set the username and password for the corresponding employee.
F1.1.3	When the admin clicks the delete icon, a pop up box will raise asking the admin “Are you sure you want to delete the employee id num# “.
F1.1.4	If the admin clicks the no button, the employee won't be deleted from the database and will be still visible to the users of the application.
F1.1.5	If the admin clicks the yes button the employee flag will be set to inactive in the database and the employee won’t be visible to the front-end user. 
F1.1.6	When the admin clicks the edit button the admin can edit and update the selected employee details and its stored to the database.


 
Req.ID	Description	Priority
 F1.2	 Adding an employee	 High
 F1.2.1	 When the admin clicks the add employee button a new page opens asking the admin to enter the new employee details like first name, last name, gender, DOB, qualification, Availability, mobile number.
 F1.2.2	If the admin enters a number in the name area, the application won't allow the admin to submit and a message shows saying the name will only accept characters.
F1.2.3	If the admin enters a character in the mobile number, the application will not allow the admin to submit and will display an error message saying “ mobile number cannot contain character”.


F.2 Clint Details

Req.ID	Description	Priority
 F2.1	 View Client details	 Medium
 F2.1.1	 When the admin clicks the client list button, the application will list all the current Client on the webpage.
 F2.1.2	 When the admin clicks the delete icon, a pop up box will raise asking the admin “Are you sure you want to delete the Client  id num# “.
F2.1.3	If the admin clicks the no button, the Client won't be deleted from the database and will be still visible to the users of the application.
F2.1.4	If the admin clicks the yes button the Client will be deleted from the database.
F2.1.5	When the admin clicks the edit button the admin can edit and update the selected Client details and it is updated to the database.

Req.ID	Description	Priority
 F2.2	 Add client details	 Medium
 F2.2.1	 When the admin clicks the add employee button a new page opens asking the admin to enter the new employee details like first name, last name, gender,and DOB.
 F2.2.2	 If the admin enters a number in the name area, the application won't allow the admin to submit and a message shows saying the name will only accept characters.
F2.2.3	When the Admin clicks the submit button the new client will be added to the database

		
F.3 Adding Round	
	

Req.ID	Description	Priority
 F.3	 Adding round	 High
 F3.1	 When the Admin clicks the add round button the application displays a page to select the date of the round.
 F3.2	 When the admin selects the date, the application will allow the admin to select the the employee according to their availability.
F3.3	When the admin selects the employee the admin can start filling the visit.
F3.3.1 when the admin starts entering  the client name for the visit, the name box will automatically fetch the data from the client database and suggests the closest name according to the typed letters.
F3.3.2 If the admin enters a time period which is more than 24hrs, an error message will be displayed saying “the start time must be smaller than the end time”. 
F3.3.3 when the admin enters a valid time the minutes must be auto populated in the minutes box.
F3.3.4 when the admin clicks the add visit button a new row for the visit will be added.
F3.3.5 If the admin enters the same time or a time that overlaps any of the previous visit an error message will be displayed saying “time overlapping”.
F3.3.6 when the admin clicks the delete (X) button at the end of the visit, the visit must be deleted from the round. 
 
F.4 Email notification

Req.ID	Description	Priority
 F4	 Email notification	High
 F4.1	 When the admin clicks the submit button after creating the round, an email of the round must be sent to the assigned worker.

F.5 Edit and view round

Req.ID	Description	
 F5.1	 Edit round	High
 F5.1.1	 When the admin clicks the round list button, the application displays the list of round created.
F5.1.2	When the admin clicks the edit button of the particular round the admin should be able to edit and update that particular round.
F5.1.3	When the admin clicks the update button the round must be updated and the email should be sent to the assigned worker again.


Req.ID	Description	
 F5.2	 View round	Medium
 F5.2.1	 When the admin clicks the view round button, the application allows the admin to select the date of the particular round.
F5.2.2	When the admin clicks the next button the application will display all the round for that particular date.
F5.2.3	When the admin clicks the eye icon the admin can view that round with all the visits .
F5.2.4	When the admin clicks the print button a pdf format of the round with its visit will be downloaded. 



Worker functional requirements
F.6 View rounds

Req.ID	Description	
 F6.1	View round	High
 F6.1.1	 When the worker clicks the view round button the application will allow the worker to search his rounds by date .
F6.1.2	When the worker is done with the visit the worker can check the done checkbox.
F6.1.3	When the worker is not able to attend a visit, the worker can give the FTA (fail to attend reason) that will be updated to the admin.

F.7 Round list

Req.ID	Description	
 F7.1	 Round list	Medium
 F7.1.1	 When the Worker clicks the round list button the application will display all the round of that worker.
F7.1.2	When the worker clicks the eye icon of the round, it displays the visits of that round.
F7.1.3	When the worker clicks the print button, a PDF format of that round will be downloaded.


NON FUNCTIONAL REQUIREMENTS SPECIFICATION
Accessibility 
	The application is accessible in multiple platform and to multiple types of users. 
Scalable 
The application is scalable and can be improved in the future with multiple features and new technology.
Performance
The application has passed in all various performance testing with good response time and throughput and has no performance issues.
Modifiability
The application developed is modifiable and the effort required to modify the application will be minimum.
Portability
	The application build is portable.
Reliability
The application has run in the server without any failure. Hence the application will be reliable if there are no server issues.
Usability
	The application is simple for the user to operate and navigate. The learning time of the application for the user will be bare minimum.




4 Architecture
	 



5          Technical framework
	5.1      ANGULAR JS MATERIAL: Angular material is a UI component library used along with Angular JS that helps in  constructing attractive, functional, faster and much responsiveness website, Since these features are our key requirements in the project, Our ideal choice was to go with Angular JS Material UI framework. Some of the key advantages of using angular material are as follows.

		         Material Design: The material design provides better experience, When the webpage is access across multiple devices like (mobile, tablet, laptop). It has a incredibly intuitive layout design to achieve our goal.
 
		         Date picker: It plays a major role in web rostering application, As the workers are assigned rounds every day. This feature is easy to implement using Angular material.
             
         Autocomplete: The feature adds great user experience to the user. It 
Provides user with an options to choose the words as he types. This feature was helpful in  
Auto populating the client name, When the user tries to add a visit for the client.

		         Input validation: It is easy to validate our input fields. For example fields like(Name, age, dob, address). It displays the error message if its not valid.

	                     Side Navigation: It was useful while creating rounds navigating from left to right with a button click and keeping mobile responsiveness of the application in mind.

      5.2  SPRING BOOT:  It is a easy framework for server side programming and deployment. Some of the advantages of using spring boot for development are:

●	Reduces development time and increase productivity.
●	It reduces boiler plate codes.
●	It provides embedded HTTP servers that was helpful in testing our web application easily
●	Maven dependencies- It reduced time for implementation and installation.
●	Avoids XML configuration.

5.3 SPRING HIBERNATE: It is an ORM framework.  In simple terms database tables are mapped as java objects immediately. Some of the advantages of using spring hibernate in web rostering application are:

		         Database independent:  It is database independent and it can be easily migrated from one database to another. It also takes care of changes made to database.

		         Scalability: It is highly scalable and can adapt itself to any environment and also can interact with large number of users at a time.

		         Dual layer caching: Hibernate support two level of caching namely first level and second level of caching. First level deals with session object and second level deals session factory object. It retains the object in the cache to avoid repeated hits in the database.
 
5.4   VISUAL STUDIO CODE:

●	VS code was used to run the angular( front-end of the application).
●	It saved plenty of time by running node JS scripts in the inbuilt terminals.
●	Inbuilt debugging console was helpful while programming and testing.
●	It had built in version control to Git

5.5  BOOTSTRAP: 

●	It is compatible with browsers like google chrome, internet explorer, firefox, safar, etc.,
●	It was very easy to set up table layout and implement the rostering table with angular.
●	Based on the device used it adjusts the web page characteristics dynamically.
●	It is easy to develop and saves coding effort by using less CSS functionality by using  pre-built blocks of code.


5.6  SLACK: 

●	Easy and professional way of communicating as a channel and private.
●	Supported all formats of our document and made it easy to send and share among the groups
●	Follow up on day to day tasks.

6          Implementation


Step1: Install spring tool kit and import the Visit folder as a maven project.
Step 2: Install MS SQL server and SQL server configuration and import the file rmit_visit_db_2 to MS SQL server.
Step 3: Open application properties in spring (src/main/resources) and set the database name and update the username password.

 



Step 4: Open Visual studio code and import the folder hospital-round visit. Also make sure Node js is installed in your system.


 



Step 5: Run the application in the terminal using the (ng s -o) command, where the application will automatically start in your default browser. 


Step 6: The admin can login using the pre-set username (admin) and password (pass).
7          Deployment Instructions
Step 1: Generate a .war file of the build from spring-boot and use ng build command for front end to generate the build.
Step 2: Use git to navigate to the folder and login using your Heroku CLI.
Step 3: Install Heroku CLI deploy.
Step 4: Install Heroku CLI deploy plugin 
Step 5: Deploy the app on Heroku: deploy target /<project name>.war – app <Heroku app name>
Start 6: Open Heroku app to start the application.
 

 

 
8          Test specifications
 
The test cases below were created based on our requirement. Some of the repeated test cases were automated to save our testing effort.

 TEST FRAMEWORK:  We used Selenium Web driver with python to automate some of our repeated process to save time.

  Advantages of using selenium web driver:
•	It is an open source tool
•	Widely recognized for web application testing.
•	Saves our manual testing effort and can be easily integrated with Pycharm.
•	Reduced our testing effort by running automation on repeated test case scenarios.


Test Cases:

Test ID	Action	Inputs(Type)	Expected Output	Actual Output	Test Browser	Test Result	Testcase type
1	To verify if the user is able to login with valid username and password	Enter valid user and password created	The user should be able to login to the application	The user was able to successfully login	 Internet
explorer	Passed	Positive
2	To verify if the user is able to login with invalid username and password	Enter username: *(&%$
  Password: 00000	Address is updated after entering and submitting	Address is updated after entering and submitting	Google 
Chrome	Passed	Negative
3	To verify if the user is able to login with blank username and password fields.	Leave the username and password fields blank	It should throw an error message saying 
”Please enter username and password to login”	The error message was successfully thrown to enter valid username and password	Mozilla    firefox	Passed	Negative
4	To verify if the user is able to add an employee and enter the valid details in the input fields	Add employee details and click on submit	The details should be successfully submitted and added to the database(MS sql)	The details are successfully registered to the database	Google 
Chrome	Passed		  Positive
5	To verify if add employee fields accepts invalid inputs	Enter name, mobile with combination of string and numbers	Error message should display saying name  cannot contain numbers and mobile number should contain only numbers.	The error messages are displayed successfully on entering invalid name and mobile number.	Internet 
Explorer	Passed	Negative
6	To verify if the added employee can be viewed in the employee list

	Click on employee list tab to view the list of employees	The added employee should be displayed in the list	The added employee should be successfully displayed in the list when clicked the list	Mozilla firefox	Passed	Positive
7	To verify if the added employee can be deleted	Click on “X” to delete the employee from the list	The employee should be deleted and a confirmation message dialogue box should appear to alert user when performing the action	The employee was successfully deleted and error message dialogue box appeared saying that “are you sure you want to delete this employee”	Mozilla 
firefox	Passed	Positive
8	  To verify the dashboard if it shows only the active employees excluding the deleted employees	After deleting the employee go back to home to check if the employee count on the dashboard is updated	The dashboard count for employees should be update for eg: 5 to 4 if one employee is deleted	The employee dashboard was successfully updated after removing an employee	Internet 
explorer	Passed	Negative
9	To verify if an user is able to add a round for an employee	Click on add round tab and select the date for assigning round to the employee	Round for that particular day should be assigned to the employee selected from the checkbox	Round was added successfully by using checkbox for selecting the employee.	Chrome	Passed	Positive
10	To verify if the calendar is disabled, if an user tries to add rounds for the past dates. For eg: (if today is 4.5.19 and the user tries to create an round for 2.5.19.)	Click on add round and try to select invalid date	The dates for days passed in the year should be disabled.	The dates for the days passed are successfully disabled.	Chrome	Passed	Negative







   11	To verify if the client name is auto populated when adding visit for an employee	Click on add round->select date->select employee->add client details.	The client name when entered “A” should auto populate suggestions of clients names with “A”	The client name when entered “A” successfully listed names that are starting with “A”.
	Internet 
Explorer	Passed	Positive
   12	To verify if client name and address accepts only valid inputs like characters and strings.	Click on add round->select date->select employee->add name and address 	The client name should  accept only characters as input and address as string format only.	The client name successfully accepted only characters and address as only strings. 	Mozilla
	Passed	Positive
   13	To verify if error message appears when entering invalid client name and address	Click on add round->select date->select employee->add name and address 	The client name and address should throw an error message saying. “name should accept only characters and address should accept only strings as input”	On entering invalid input. Error message was displayed saying client name can contain only characters and address can contain only strings.	Internet explorer	Passed	Negative
   14	To verify if the error message is thrown while entering invalid time. For eg: start time: 8:00 end time: 7:00.	Click on add round->select date->select employee->add start time->end time	The start time and end time should throw an error message if the timings are invalid	The error message was thrown successfully while entering invalid time as input	Chrome	Passed	Negative
 15	To verify if the application accepts valid time for visit.	Click on add round->select date->select employee->add start time->end time	The start time and end time should not throw any error while adding visit for the client	The visit was successfully added for the client	Chrome	Passed	Positive
 16	To verify if the time overlap error message is thrown while entering same time for multiple clients	Click on add round->select date->select employee->add start time->end time	The start time and end time should throw a time overlap error message when entering same time for multiple employees	The time overlap error message was thrown successfully when entered same time for multiple clients visit.	Mozilla	Passed	Positive
 17	To verify if the round is updated in round list tab.	Click on round list to view if the list is updated with the new round added	The employee name with visit details should be updated in the list.	The employee name and visit details of the client was successfully added.	Internet explorer	Passed	Positive
 18	To verify if the round can be deleted	Click on round list to view if the list.	The round should be deleted successfully	The round was successfully deleted	Chrome	Passed	Negative
 19	To verify if the round details can be modified 	Click on round list to view if the list.	The user should be able to modify the round.	The user was able to modify the round successfully	Mozilla	Passed	Positive
 20	To verify if the admin is able to add default client	Click on client list->add client	The user should be able to add client successfully	The user was able to add the client successfully	Internet explorer	Passed	Positive
 21	To verify if the email notification is triggered and displays the details of the shift.	The shift details should be displayed in table in the email.	The employee should be able to get the email notification regarding the shift details via email.	The email notification was successfully received via email.	Chrome	Passed	Positive
 22	To verify if the admin can export the roster into printable PDF format.	After adding the visit details click on print button in the bottom to export the roster details to PDF format.	The roster should be download and be able to open.	The roster was successfully downloaded and exported to PDF format.	Mozilla	Passed	Positive
 23	To verify if error message is thrown when trying to download an empty roster	Leave the visit field blank and click on print button in the bottom to export the roster details to PDF format.	The error message should be thrown saying that “please the enter the details”.	The error message was successfully displayed	Internet explorer	Passed	Negative
 24	To verify if the minutes are auto populated while entering the start time and end time.	Enter start time and end time observe the minutes column to see if the minutes are calculated with respect to the time entered.	The minutes should be calculated automatically when the start and end time is entered.	The minutes was auto populated successfully.	Chrome	Passed	Positive
 25	To verify if the user is able to log out successfully.	Click on log out tab to check if the user is able to log out gracefully.	On clicking log out the user should be able to log out of the application	The user was successfully able to log out of the application	Mozilla	Passed	Positive
 26	To verify if employee is able to sign in and view his shift details	Enter username and password and click on view round tab to check the roster details.	The employee should be able to view his shift details on clicking the view round tab.	The employee was able to successfully view his shift details.	Mozilla	Passed	Positive
 26	To verify if the employee was able to confirm the shift by clicking the checkbox and get updated to the admin. 	Click on view round and click on checkbox and submit. The confirmation should be updated in the admin round list.	The confirmation should be updated in the admin round list.	The employee confirmation was updated successfully in round list.	Internet explorer	Passed	Positive
 27	To verify if the FTA reason is disabled on clicking the done checkbox.	Click on view round->click on done checkbox.	The FTA reason should be disabled.	The FTA reason was successfully disabled.	Chrome	Passed	Negative
 28	To verify if the employee FTA reason was successfully updated to the admin, in case if he fails to attend the shift.	Click on view round->and type the FTA reason field.	The FTA reason when updated should be updated to the admin round list.	The FTA reason was successfully updated when entered by the employee.	Internet explorer	Passed	Positive
 29	To verify if employee is able to print the roster.	Click on print button to export the roster.	The print button should be able to export the roster  	The roster was successfully exported by the user	Mozilla	Passed	Positive
 30	To verify if employee is able to log out of the application	Click on log out tab	The employee should be able to log out of the application	The employee was successfully logged out of the application.	Chrome	Passed	Positive

9          Testing Results

  


	      As you can see in the above pie chart. The defects are classified into two categories:
•	Functional defects
•	Usability defects

They are further classified based on the priority and severity of the defects.


      Functional defects: As you can see the graph more than 50% of the defects found were related to functionality of the software. Most of defects were encountered while creating rounds for the employees. Especially with time functionality. Multiple times we faced issue while creating rounds which is the core part of the project and clearly a ship blocker. These issues were tested and fixed in the later sprints. The functional issues contributed more in priority and severity list of defects.

      Usability defects: We encountered few critical user interface issues and most of the issues were clipped strings, misalignment and scroll bar issues.

     We have further categorised both functional and usability issues into priority and severity based on the impact it created.

      Priority 1 & severity 1: We have classified the ship blocker issues into priority 1 and severity.  Basically the defects which we felt had more impact on the customer who uses the application. Most of the P1 & S1 defects were functionality issues.

      Priority 2 & severity 2: We have classified the issues that had less impact on the customer into P2 & S2 by which the application can be still released with less impact on the functionality.
