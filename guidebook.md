# Lab 0: Introduction

## Goal
The Story Testing Scripts Scoped Application lab will guide users on how to use ServiceNow&reg; Studio IDE to build out a custom application that helps create test scripts for stories. Developers are often confused on what requirements are needed by the quality assurance team for testing. This will break down the test script process into what users they should be impersonating, the steps they should be taking and more. This lab will go over what should be included in a best practice test script and how to build a scoped application to record test scripts in ServiceNow instead of in Excel or another system. This lab will touch developers on Studio IDE, story best practices, scoped applications, and process improvement.

# Lab 1: The Fundamentals of Testing Scripts
Explain the different terminologies and overall scenario. < directly from ATF > 
## What are testing scripts and why should I use them?
< ATF  or itil library >
< Note that we turned on Agile Development 2.0 to build app >
## Planning the layout of our application

# Lab 2: Starting with ServiceNow&reg; Studio IDE

## Create the Scoped Application

1. Navigate to **System Applications > Studio.**  
![](images/nav_studio.png)

2. Click the **Create Application** button.  
![](images/select_application.png)

3. Click the **Let's get started** button on the "Welcome to the new way to set up your apps"

4. Fill out the following values on the "General Info" tab:

**Name:** Story Testing Scripts  
**Description:** Create testing scripts for stories.  
**Scope:** x_441376_sts (Note, your instance may have a different number.  

5. Drag the "checkbox.png" image from the lab files to the "Drag or drop" icon area.

6. Verify all the information is correct and click **Create**  

7. On the "Let's create some roles for this app", click the **+Create new role** 

8. Enter in "test_script_user" in the "New role name" field and click **Create**  
![](images/test_script_user_role.png)

9. The role should now appear in the "Roles" list with the scope in front of it.
![](images/test_script_role_added.png)

10. Click **Continue** to go to the next step.

11. Our application will be used on stories in the classic view of ServiceNow. Select **Classic** and click **Continue** to go to the next page.  
![](images/select_classic_view.png)

12. You should now see the "Which data tables do you want to use for this app?" We will be building out new tables based on the arhitecture we mentioned previously in lab 1. Click on **Create new table**.  

13. On the next screen select the **Create table from scratch** and click **Continue**.  
![](images/create_table_from_scratch.png)

14. We will be createing a table for the test scripts first. Go ahead and click **Add a new field** and put in the following:  
![](images/adding_fields_to_test_script_table.gif)  


Add the following fields to the Test Script table:

Field Label | Field Name | Type | Length | Reference
------------ | ------------- | ------------- | ------------- | -------------
Name | name | String | 40 |
Description | description | String | 1000 |
Story | story | Reference | 32 | rm_story
Tested By | tested_by | Reference | 32 | sys_user
Reviewed By | reviewed_by | Reference | 32 | sys_user
Version | version | Integer |  | 
QA Tester's Notes | qa_tester_s_notes | String | 1000
Reviewer's Notes | reviewer_s_notes | String | 1000

15. Click **Continue** after you have added all the fields to the table.

16. Now we will name the table the following:

![](images/test_script_table_name.png)

**Table label:** Test Script  
**Table name:** x_441376_sts_test_script (Your instance may have a different number in the table name.)
**Make extensible:** true

17. Click the **Continue** button to create the table. It may take the system a few seconds to create the table.

18. You should see a "Success! Your table is ready" screen. Click on **continue** to build the Scenario table next.

![](images/test_script_table_is_ready.png)


Add the following fields to the Scenario table:

Field Label | Field Name | Type | Length | Reference
------------ | ------------- | ------------- | ------------- | -------------
Name | name | String | 100 |
Prerequites | prerequites | String | 1000 | 
Personas | personas | String | 1000 | 
Company | company | Reference | 32 | core_company
Test Scenario | test_scenario | String | 1000 | 


Add the following fields to the Test Steps table:

Field Label | Field Name | Type | Length | Reference
------------ | ------------- | ------------- | ------------- | -------------
Number | number | String | 40 |
Description | description | String | 1000 |
input variables | prerequites | String | 1000 | 
Expected Results | expected_results | String | 1000 | 
Company | company | Reference | 32 | core_company
Actual Result | actual_result | String | 1000 | 
Result State | result_state | Select Box |  | 

Result State choice list:

Label |  Name | Type 
------------ | ------------- | ------------- 
Pass | pass | String 
Fail | fail | String 
Suspended | suspended | String 
Not Tested | not_tested | String 




# Lab 3: How to change the layouts

# Lab 4: Recording Test Scripts

# Lab 5: Best Practices
## How to create successful testing scripts. 

# Lab 6: Extra Credit

## How to publish my scoped application to an update set

## How to publish my scoped application to the ServiceNow&reg; Share

## Other areas to expand the Testing Scripts Scoped Application. 

