QA Technical Test Assignment
SoapUI Automation framework using free version of SoapUI. No need of SoapUI paid version.


Getting Started:
Download REST Project 2-soapui-project.xml. 
Import REST Project 2-soapui-project.xml in SoapUI tool.


Verify the imported project in SoapUI:
There will be only one project (REST Project 2), one testsuite (TestSuite) and two test cases (Happy path test and Negative test). And Happy path test case include a few steps.All test steps in Happy path test should be in this sequence:


GETALL step: get all the data through REST service and verify REST service response status, valid HTTP Status Codes and service response time.

GET step: get data according to the expected userId and verify the searching results which have the same userId, valid HTTP Status Codes and service response. time

POST step: create data and verify created data with expected data, REST service response status, valid HTTP Status Codes and service response time.

PUT step: update data and verify created data with expected data, REST service response status, valid HTTP Status Codes and service response time.

DELETE step: delete data according to the testSuite level variable ID

End

And Negative test case only has one step (Request 1), it verifies the reponse is empty.


Notice:
Due to the some giving resources are the same, each step make sure to choose the right resource/method. In default, the downloading file imported in Soup UI, GET Step and DELETE Step have to choose right resource/Method to run.

Running the tests:
You can run the test directly from the SoapUI tool.

Summary:
All the variables and url resources are stored in the testsuite level. When designing more tests, we can change variables easily on the testsuite level so that it increases the scalability of solution. And the verification and validation methods or business logic are stored in each test steps which can be flexiable to maintain and recycle the code in future.

Author:
Furong(Don) Huang
