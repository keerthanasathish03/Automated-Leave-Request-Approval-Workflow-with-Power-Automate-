# Automated-Leave-Request-Approval-Workflow-with-Power-Automate-
## Overview
This Power Automate flow automates the employee leave request and approval process. It integrates Microsoft Forms for request submission, SharePoint to track leave requests, and Power Automate approvals for management decision-making. The flow updates leave statuses based on approval outcomes.

## Features
- Captures leave requests using Microsoft Forms.

- Creates and updates SharePoint list items for each request.

- Starts an approval process for each leave request.

- Updates the request status in SharePoint to Approved or Rejected.

- Sends email notifications and calendar events (planned but not implemented due to Outlook access restrictions).

## Flow Summary
1. Trigger: When a new response is submitted in Microsoft Forms.

2. Action: Get response details from the form.

3. Action: Create a new item in SharePoint list with leave request details.

4. Action: Start and wait for an approval.

5. Condition: Based on approval outcome, update item status to Approved or Rejected in SharePoint.

## Prerequisites
- Microsoft Power Automate account with necessary licenses

- Access to Microsoft Forms for submitting requests

- SharePoint Online site with configured list for leave requests

- Optional: Outlook/Microsoft 365 access for email/calendar (currently not available)

## How to Use
* Import the exported flow package into your Power Automate environment.

* Connect necessary services like Microsoft Forms, SharePoint, and (optionally) Outlook.

* Customize SharePoint list and form as needed.

* Run the flow by submitting leave requests via the linked Microsoft Forms.

## Known Limitations
- Email notifications and calendar event creation are designed but not yet implemented due to lack of Outlook access.

- Tested primarily in specific environments/sample data conditions.

## Additional Resources
+ SharePoint list columns: EmployeeID, EmployeeName, LeaveStartDate, LeaveEndDate, Reason, Status.

+ Microsoft Forms structure for leave request capturing.

+ Planned email and calendar integration when Outlook access is available.

## Import Instructions
- Download the exported flow package (zip file).

- Login to Power Automate.

- Navigate to My Flows > Import.

- Upload the zip package and map required connections (Forms, SharePoint).

- Complete import and save the flow.

- Test it with sample leave requests.

<img width="277" height="412" alt="image" src="https://github.com/user-attachments/assets/c8b68226-685b-4067-b168-be094220fb48" />
<img width="319" height="437" alt="image" src="https://github.com/user-attachments/assets/1e40001c-4942-4cbb-952b-e26790fc540e" />
<img width="860" height="137" alt="image" src="https://github.com/user-attachments/assets/98725208-0472-46c2-a0fd-b7d6f7766aed" />



