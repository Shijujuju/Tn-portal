Project Demonstration
1. Introduction
The project demonstration explains the working of the automated laptop procurement system developed using ServiceNow Flow Designer. The system simplifies the process of placing laptop requests, obtaining approval, and automatically generating configuration tasks for the Hardware team.
2. Demonstration Steps
Step 1: Open Service Catalog
The ServiceNow Service Catalog provides different categories such as Hardware, Software, Services, and Office. The user navigates to the Hardware category to access laptop-related services.
Step 2: Select Standard Laptop
The user selects the Standard Laptop item from the Hardware category. The catalog displays the laptop details and allows the user to proceed with the order.
Step 3: Submit Laptop Request
The user clicks Order Now to submit the laptop request. ServiceNow generates a unique request number and creates the corresponding request record.
Step 4: Approval Process
The submitted request is processed through the approval mechanism. Once approved, the automated workflow is triggered.
Step 5: Automated Task Creation
The Standard Laptop Task flow executes using Flow Designer. The Create Catalog Task action automatically generates a configuration task for the requested laptop.
Step 6: Task Assignment
The generated Catalog Task contains the updated short description and is assigned to the Hardware assignment group for further configuration.
Step 7: Verify Output
The user opens the Requested Item record and checks the Catalog Tasks section to verify the generated task, description, and assignment group.
3. Expected Output
Successful submission of a Standard Laptop request.
Approval of the service request.
Automatic creation of a Catalog Task.
Automatic assignment to the Hardware team.
Updated task description.
Improved tracking of laptop configuration activities.
4. Result
The demonstration verifies that the ServiceNow Flow Designer automation works as intended. After approval, the system creates a Catalog Task and assigns it to the Hardware group, reducing manual intervention and improving procurement efficiency.
5. Conclusion
The project demonstration successfully illustrates the automation of standard laptop procurement using ServiceNow Flow Designer. The implementation streamlines request processing, improves task allocation, minimizes delays, and enhances the overall efficiency of IT procurement operations.

DEMO VIDEO LINK:https://drive.google.com/file/d/1DTb76yGKvJTFhCl926qasxOpcQfptE9U/view?usp=drivesdk

Summary

The project focuses on streamlining the IT procurement process by automating standard laptop orders using ServiceNow Flow Designer. The existing manual process often causes delays, additional workload, and errors in laptop configuration task assignment.
The proposed solution uses a Service Catalog trigger and the Create Catalog Task action to automatically generate configuration tasks after approval of a Standard Laptop request. The generated task is assigned to the Hardware group with the required short description and approval details.
The workflow reduces manual intervention, improves task allocation, minimizes user waiting time, and enhances the overall efficiency of IT procurement operations. The implementation provides a more organized and automated approach to handling standard laptop requests.

Conclusion

The project successfully demonstrates the use of ServiceNow Flow Designer to automate standard laptop procurement and configuration tasks. By integrating the Service Catalog with an automated workflow, the system ensures that configuration tasks are generated and assigned to the Hardware team after request approval.
This automation reduces manual workload, minimizes processing delays, improves resource utilization, and enhances the user experience. The project provides an efficient and reliable approach to managing standard laptop orders within the IT department.
Overall, the implementation achieves its objective of improving IT procurement efficiency through workflow automation and demonstrates the practical application of ServiceNow Flow Designer in streamlining IT operations.



