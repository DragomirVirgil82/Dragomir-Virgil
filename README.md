# Dragomir-Virgil
Manual Testing_Proiect
# Final Project for IT Factory Manual Testing course

The scope of the final project is to use and show all the knowledge I have learned through the course and from self research and to apply them when using a live application.
* Application under test: [XYZ Bank](https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login)

I have created my own documentation in order to find bugs and static testing issues. The application comes without any original documentation.
* Documentation: [Documentation for XYZ Bank](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/Documentatie%20pt%20xyz%20bank.docx).
* API documentation: [Simple Book Api Documentation](https://github.com/vdespa/introduction-to-postman-course/blob/main/simple-books-api.md)

The final project will be split into 2 sections: **Testing section** (where tracking process will be done in Jira and Zephyr tools) and the **SQL Section**. The testing section will also contain  2 section, GUI testing and Api testing that will be done in Postman tool.
     
Tool used: **Jira, Zephyr Squad, Postman, SQL Workbench, Github.**

# Functional Specification
* The business requirments can be found [here](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/Documentatie%20pt%20xyz%20bank.docx).

The **XYZ Bank** application is an application created for the usability both of the costumers and the bank manager. With this app the customer should be able to check his bank account and see the transactions that the customer has made over one period, the credit balance and he can deposit or withdrawal money to and from the customer bank account.
![image](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/7ff69070-bc54-416d-8f65-1ff843a7fe48)
![epic2](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/fbcb1abe-798e-44f6-9e13-85f5fb5e823f)
![epic 2 1 1](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/170d50f5-8e00-4a15-acb0-d879ad8b75ce)
# **1. Testing Section**
## **1.1. Test planning**
* The Test Planning is designed to describe all the details of the testing of the [XYZ Bank application](https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login)

This section - test planning -will identify the items that will be tested, the futures to be tested, the types of the testing that will be performed and it will also define the entrence and exit criteria that needs to be completed, the assignee roles for the project and all the human resorces that will be in charge. 
The testing allocated time and financial resources will be defined, along with the risk associated with the plan.

#### 1.1.1. Roles assigned for the testing project and the human resource 
* Scrum manager - dragomirvirgilcatalin82
* Software Tester - dragomirvirgilcatalin82
* Review leader - dragomirvirgilcatalin82
* Software architect - Jane Doe
* Developer - Jane Doe
#### 1.1.2. Entry criteria defined
* Roles and human resource are alocated
* The sistem is up and running
* User is created
#### 1.1.3. Exit criteria defined
* All test cases created are executed
* At least 75% of the executed test cases have the status passed
* There is a maximum of 4 high rated bugs opened and they are assigned to the developer to be fixed
* There is a maximum of 10 open bugs and no critical bug can be opened.
* The regression test needs to be done
* Testing deadline 30.06.2023
#### 1.1.4. Test scope
* Test in scope: Review and functional testing using black box, test design techniques based on experience testing, GUI testing, regression testing, Api testing
* Test not in scope: Non-functional testing - Performance Testing, Stress testing, Volume Testing, compatibility testing with multiple browsers, Mobile testing  and Functional Testing using White-box Testing Tehniques. 
#### 1.1.5. Risks detected
* Project risks: developers not availabe to develop the app on time to be testing and fix the finded bugs, vacancy, lack of people, non functional environment, illness, too many juniors both testers and develpers;
* Product risks: operational risk, validation risk, price risks, poor usability and quality of the application.
#### 1.1.6. Evaluating entry criteria

The entry criterias defined in the Test Planning phase have been achieved and the test process continued.

## ** 1.2. Test Monitoring and control**

It was done by generating periodic reports that reflect the current status of the tests.

![Jira board print 1Untitled](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/63d0395b-b837-466e-b4a9-ff6c5eeead30)

![TEST CASES](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/7ca93a57-bb85-48bd-9cb6-2846ae7536d0)

![Run Collection Postman](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/POSTMAN%20RUN%20COLLECTION.jpg)

## ** 1.3. Test Analysis**
* The above [requirements](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/Documentatie%20pt%20xyz%20bank.docx) were reviewd for the Ui testing and for the Api testing I've followed the [documentation]() and work with it.
* 
!During the review, some defects were raised and you can check them here:![MTFP-36](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/a41ecfdc-2f5c-4d68-a49d-67cbc10ba7ef)

* After the defects was fixed, a new documentation was release as you can check here: [New documentation for  xyz bank.docx](https://github.com/dragomirvirgilcatalin82/manual_testing_project/files/11713229/New.documentation.for.xyz.bank.docx) and the testing process was executed and following the test conditions above:

* Check if you can login into the application;
* Check if the bank manager can add a customer;
* Check if the bank manager can open an account;
* Check if the new customer is added to the customer list;
* Check if the bank manager can delete a customer;
* Check if the customer can login;
* Check if customer has a list with his transactions;
* Check if customer can see transactions between a period known;
* Check if customer can make a deposit;
* Check if customer can make a withdrawal;
* Check if new currency can be added;
* Check add, delete, reset actions via Ui;
* Check the Post, Get, Patch, Delete for the Api testing using Postman tool;
## **1.4. Test Design**
Functional test cases were created in Zephyr Squad. Based on the analysis of the documentation, the test case design used for generating test cases are:
* Black box testing - use testing;
* Experience based testing: exploratory testing and check list based testing.
*Test cases:*
* [MTFP-65] Verify if a customer can make more then 2 withdrawals/24 h
* [MTFP-64] Verify if a customer can withdrawal an amount that is less then his current balance
* [MTFP-63] Verify if a customer can withdrawal a bigger amount then his bank current balance
* [MTFP-62] Verify if a customer can make a 0 value deposit
* [MTFP-61] Verify if a customer can make a deposit with minimum 1 Euro of the equivalent of 1 Euro
* [MTFP-60] Check if the customer can go back to the Home menu by pressing the Back button
* [MTFP-59] Verify if a customer can reset all his transactions using the Reset button
* [MTFP-58] Check if you can select a date-time from the calendar to show the transactions details
* [MTFP-57] Verify if the Transaction subsection has all the required fields inserted
* [MTFP-56] Check if the customer can logout from the app using the Logout button
* [MTFP-55] Verify if the customer can login into the XYZ Bank app
* [MTFP-53] Verify if you can Delete a customer from the database using the Delete button
* [MTFP-52] Verify if the Customer subsection has all the required fields inserted
* [MTFP-51] Verify if you can search a customer into the search customer field, Customers subsection, Bank Manager section
* [MTFP-48] Verify if you can open an account entering valid customer and a currency
* [MTFP-47] Verify if you can open an account without selecting a currency
* [MTFP-46] Verify if you can open an account without selecting the customer
* [MTFP-45] Verify if open account is possible in any currency that are in use in the world at this time
* [MTFP-44] Verify if the Open Account subsection has all the required fields
* [MTFP-43] Verify if you can add customer duplicating another that already exists
* [MTFP-42] Verify if you can add a customer without complete the Post Code field
* [MTFP-41] Verify if you can add a customer without complete the LastName field
* [MTFP-40] Verify if you can add a customer without complete the First Name field
* [MTFP-39] Verify if you can add a customer using valid details
* [MTFP-37] Verify if the Add customer subsection has all the required fields
* [MTFP-33] Verify if you can login into the XYZ bank app in the bank manager section

 #### All the test cases with steps can be viewed here: [ZFJ-issue-export-06-12-2023-242ac113-0001.xlsx](https://github.com/dragomirvirgilcatalin82/manual_testing_project/files/11735657/ZFJ-issue-export-06-12-2023-242ac113-0001.xlsx)

#### Api Test Cases:

* [GET] API Status
* [GET] Negative testing - Api Status
* [POST] API Clients 
* [POST] Negative testing - API Clients 
* [GET] List of books
* [GET] Single book
* [GET] Negative testing - Single book
* [POST] Order book
* [POST] Negative testing - Order book
* [GET] Get all book orders
* [GET] Negative testing - Get all book orders
* [GET] Get an order
* [GET] Negative testing - Get an order
* [Delete] Delete order
* [Delete] Negative testing - Delete order


#### All the Api test cases using Postman tool can be viewed [here](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/Simple%20Book%20API.postman_collection.json)

## ** 1.5. Test implementation
The following elements are needed to be ready before the test execution phase begins:
* Roles and human resources are alocated
* The system is up and running : [environment](https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login)
* Both bank manager user and customer user are created: customer user: dragomirvirgilcatalin82/ bank manager account - user: John Malkovici/ password: johnswife1
* Cycle summary was created
* Test cases were added to the cycle summary
* Postman collection with the dependents API methods was created
* Authorization token was created for accessing the API.

## ** 1.6. Test execution
Test cases are executed on the created test Cycle. Check summaries bellow:

![cycle summary](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/0163d28a-eb1f-402e-8ccb-7ef1bd8242eb)

Due to the test cases executed, bug reports has been created.
Bug report example:
![BUG REPORT EXAMPLE](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/8467cce6-bf77-4030-b752-89820c82ce4e)
![BUG REPORT 2](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/619a8cbb-b494-4cfb-b352-244a3ae18e3e)

Bug report list:

![Bug table](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/ef11e0e2-c77b-4042-b8fe-60c28c20ca8b)

*Full regression testing is needed after the bugs are fixed.*

* API tests were written in Postman and contains GET, POST and DELETE HTTP methods. You can check collection and environment With GET token call i stored the bearer token into a variable as current value to be sure will not be shared or stored in cloud.

* All calls contain few tests too. The tests are checking: returned status (as 200 or 400/404 for negative tests) and the response body. For more details please import collection [here](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/Simple%20Book%20API.postman_collection.json)

## **1.7. Test completion
* All the exit criteria has been passed.
* There are no more then 4 bugs with high severity and priority open
* 78% of the executed test cases have the status passed
* There were created and executed 26 test cases
* Acording to the execucted test cases, 8 bugs were found and bug's reports were created
* The [Manual Testing Final Project Backlog](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/Jira.csv)
* The traceability matrix was created and can be found here: 
[Forward Traceability_13_6_2023.xlsx](https://github.com/dragomirvirgilcatalin82/manual_testing_project/files/11736140/Forward.Traceability_13_6_2023.xlsx)

![traceability matrix ook ](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/2ab84a13-b9ce-4b74-9c2c-837d205318ee)
* The traceability matrix per story example:
![traceability matrix per story ok 2](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/514932fb-af65-4bab-aa30-578e2c04a94f)

The Dashboard was created and you can see it below:
![DASHBOARD](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/afa88e2d-f241-4dad-9a21-47ccab090689)



![TEST EXECUTION](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/95a4f9d0-681f-4e68-bc31-e2d5017c5a8b)

![CREATED VS REPORTED](https://github.com/dragomirvirgilcatalin82/manual_testing_project/assets/134077299/2fc659b4-9f15-4436-8d36-5bee8e20f9c6)

![Postman Monitor](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/Monitor%20postman%20.jpg)
![Postman Run Collection negative testing](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/Run%20collection%20negative%20testing.jpg)
![Postman Run Collection negative testing](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/Run%20collection%20POstman%20negative.jpg)

# SQL Section
I have created my own database and have made same querys with it.
![SQL Diagram](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/Banking_database_schema_EER_Diagram.jpg)
* The SQL queries done for this project can be found [Here](https://github.com/dragomirvirgilcatalin82/manual_testing_project/blob/main/bank_DB.sql)
