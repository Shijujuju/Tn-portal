Project Development
1. Introduction

Project Development is the process of converting the proposed system design into a functional application. This project is developed using ServiceNow Flow Designer to automate standard laptop procurement and configuration task creation.

The system automatically generates a Catalog Task after approval of a Standard Laptop request and assigns it to the Hardware team.

2. Development Environment
Software Requirements
Platform: ServiceNow
Automation Tool: Flow Designer
Module: Service Catalog
Application: Global
Execution User: System User
Browser: Google Chrome
3. Development Process
Step 1: Create a New Flow
Open the ServiceNow platform.
Navigate to All and search for Flow Designer.
Open Flow Designer under Process Automation.
Click New and select Flow.
Enter the flow name as Standard Laptop Task.
Select Global as the application.
Set Run As to System User.
Submit the flow properties.
Step 2: Configure the Trigger
Click Add a Trigger.
Search for Service Catalog.
Select the Service Catalog trigger.
Click Done.

This trigger initiates the workflow when the relevant service catalog request is processed.

Step 3: Add Create Catalog Task Action
Navigate to the Actions section.
Click Add an Action.
Search for Create Catalog Task.
Select the action.
Drag and drop the Requested Item Record into the Request Item field.
Verify that the table is populated as Catalog Task.
Step 4: Configure Task Fields

Configure the following values:

Field	Value
Action	Create Catalog Task
Request Item	Requested Item Record
Table	Catalog Task
Short Description	Laptop need to Configured
Description	Laptop need to Configured
Assignment Group	Hardware
Approval	Approved

Leave the remaining fields as default and click Done.

Step 5: Save and Activate the Flow
Click Save.
Click Activate.
Confirm activation.

The flow is now ready to be associated with the Standard Laptop catalog item.

4. Flow Assignment
Open ServiceNow.
Search for Maintain Items.
Select the Standard Laptop record.
Navigate to Process Engine.
Remove the remaining automation configurations as required.
Add the newly created Standard Laptop Task flow.
Save the record.
5. Service Catalog Integration
Navigate to Service Catalog.
Open the Hardware category.
Select Standard Laptop.
Click Order Now to submit a request.
Open the generated request number.
Navigate to the Approvers section.
Approve the request.
6. Workflow Execution

After approval, the configured workflow creates a Catalog Task automatically.

The generated task contains:

Short Description: Laptop need to Configured
Description: Laptop need to Configured
Assignment Group: Hardware
Approval: Approved

The Hardware team can access the assigned task for laptop configuration.

7. Testing and Verification

The developed system is verified through the following steps:

Submit a Standard Laptop request.
Verify the request and approval record.
Approve the request.
Open the Requested Item record.
Navigate to the Catalog Tasks section.
Open the generated task.
Verify the short description and assignment group.
Confirm that the task has been created successfully.
8. Development Outcome

The development process successfully implements an automated workflow for standard laptop procurement. The system reduces manual task creation, ensures assignment to the Hardware group, and improves the efficiency of the IT procurement process.
