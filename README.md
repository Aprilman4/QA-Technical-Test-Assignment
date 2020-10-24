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

Property Transfer step: pass the POST step of response id and store it to the testSuite level variable ID. 

PUT step: update data and verify created data with expected data, REST service response status, valid HTTP Status Codes and service response time.

DELETE step: delete data according to the testSuite level variable ID

End

And Negative test case only has one step (Request 1), it verifies the reponse is empty.


Running the tests:
You can run the test directly from the SoapUI tool.


Author:
Furong(Don) Huang
