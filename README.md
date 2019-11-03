# InsuranceForm
The maven project contains end to end automation flow for Insurance Application

Steps to run the application:
1.Download the project.
2.Import the project as a Maven Project in Eclipse IDE.
3.Update the project to add dependencies from pom.xml.
4.Run the project as Configuration where 
a.Base Directory is the location of the project in your local machine
b.Goals will be set as: clean test -DsuiteXmlFile=testng.xml
c.Click on Run.

Framework Overview:

POM.xml to add the dependencies.
TestNg to specify the methods to be executed for the current run .It can also be used to pass the parameters
TestScripts to specify the entire flow.
Object Repository to mention the locators of the various elements (Currently implemented for login page only)
Test Data to add the test data , so as to keep it seperate and only one file would be changed (Currently implemented for login page only)
InitandDestroyClass to perform actions which are required everytime during suite execution.
Log4j integration for log generation.Logs get generated on the console and also at the location $workspace\InsuranceForm\logs

Post Script: Have tried to use different error handling techniques like try-catch, If-else,assertions. Also I have used various waits that is implicit,explicit and thread.sleep.
