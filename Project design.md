Project Design
1. Introduction

Project Design describes the structure, workflow, and components of the proposed system. The project is designed to automate standard laptop procurement and configuration using ServiceNow Flow Designer. The system automatically generates catalog tasks and assigns them to the Hardware team after approval.

2. System Architecture

The proposed system consists of the following components:

User
Service Catalog
Service Request
Approval Process
Flow Designer
Catalog Task
Hardware Assignment Group
3. System Workflow

The system follows the workflow below:

The user opens the ServiceNow portal.
The user navigates to the Service Catalog.
The user selects the Standard Laptop item.
The user submits the laptop request.
The request is sent for approval.
Once the request is approved, the Flow Designer workflow is triggered.
The system automatically creates a Catalog Task.
The short description and description are updated.
The task is assigned to the Hardware group.
The Hardware team performs laptop configuration.
The task status can be monitored through the Requested Item record.
4. Flow Design
Flow Name

Standard Laptop Task

Flow Properties
Application: Global
Run As: System User
Trigger: Service Catalog
Action: Create Catalog Task
Action Configuration
Field	Configuration
Action	Create Catalog Task
Request Item	Requested Item Record
Table	Catalog Task
Short Description	Laptop need to Configured
Description	Laptop need to Configured
Assignment Group	Hardware
Approval	Approved
5. Process Flow Diagram
        Start
          |
          v
   User Opens ServiceNow
          |
          v
   Service Catalog
          |
          v
   Select Standard Laptop
          |
          v
   Submit Laptop Request
          |
          v
    Approval Process
          |
          v
    Request Approved
          |
          v
    Flow Designer Trigger
          |
          v
   Create Catalog Task
          |
          v
   Update Task Description
          |
          v
   Assign to Hardware Group
          |
          v
   Laptop Configuration
          |
          v
         End
6. Module Design
6.1 Service Catalog Module

Allows users to select and order the Standard Laptop service item.

6.2 Approval Module

Handles approval of the submitted laptop request before task generation.

6.3 Flow Designer Module

Automates the workflow and creates a catalog task after the service catalog trigger.

6.4 Task Assignment Module

Automatically assigns the generated task to the Hardware assignment group.

6.5 Monitoring Module

Allows users to view the requested item and catalog task details, including the short description and assigned group.

7. Database Design

The project uses ServiceNow records to manage the procurement process.

Record	Purpose
Service Catalog Item	Stores Standard Laptop request details
Service Request	Maintains the submitted request
Requested Item	Represents the requested laptop
Approval Record	Stores approval information
Catalog Task	Stores configuration task details
Assignment Group	Identifies the Hardware team
8. Expected System Output

After successful execution of the workflow:

A Catalog Task is automatically generated.
The task contains the updated short description.
The assignment group is set to Hardware.
The approval field reflects Approved.
The task is available for monitoring through the Requested Item record.
