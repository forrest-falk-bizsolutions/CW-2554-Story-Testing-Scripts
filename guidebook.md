# Lab 0: Introduction

## Goal
The Story Testing Scripts Scoped Application lab will guide users on how to use ServiceNow&reg; Studio IDE to build out a custom application that helps create test scripts for stories. Developers are often confused on what requirements are needed by the quality assurance team for testing. This will break down the test script process into what users they should be impersonating, the steps they should be taking and more. This lab will go over what should be included in a best practice test script and how to build a scoped application to record test scripts in ServiceNow instead of in Excel or another system. This lab will touch developers on Studio IDE, story best practices, scoped applications, and process improvement.

# Lab 1: The Fundamentals of Testing Scripts
Explain the different terminologies and overall scenario. < directly from ATF > 
## What are testing scripts and why should I use them?
< ATF  or itil library >
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

Field Label | Field Name | Type | Length
------------ | ------------- | ------------- | -------------
Name | name | String | 100
Description | description | String | 256

# Lab 3: How to change the layouts

# Lab 4: Recording Test Scripts

# Lab 5: Best Practices
## How to create successful testing scripts. 

# Lab 6: Extra Credit

## How to publish my scoped application to an update set

## How to publish my scoped application to the ServiceNow&reg; Share

## Other areas to expand the Testing Scripts Scoped Application. 

