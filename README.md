# Automated-Leave-Request-Approval-Workflow-with-Power-Automate-
## Overview
This Power Automate flow automates the employee leave request and approval process. It integrates Microsoft Forms for request submission, SharePoint to track leave requests, and Power Automate approvals for management decision-making. The flow updates leave statuses based on approval outcomes.

## Features
Captures leave requests using Microsoft Forms.

Creates and updates SharePoint list items for each request.

Starts an approval process for each leave request.

Updates the request status in SharePoint to Approved or Rejected.

Sends email notifications and calendar events (planned but not implemented due to Outlook access restrictions).

## Flow Summary
Trigger: When a new response is submitted in Microsoft Forms.

Action: Get response details from the form.

Action: Create a new item in SharePoint list with leave request details.

Action: Start and wait for an approval.

Condition: Based on approval outcome, update item status to Approved or Rejected in SharePoint.

## How to Use
Import the exported flow package into your Power Automate environment.

Connect necessary services like Microsoft Forms, SharePoint, and (optionally) Outlook.

Customize SharePoint list and form as needed.

Run the flow by submitting leave requests via the linked Microsoft Forms.

## Additional Resources
SharePoint list columns: EmployeeID, EmployeeName, LeaveStartDate, LeaveEndDate, Reason, Status.

Microsoft Forms structure for leave request capturing.

Planned email and calendar integration when Outlook access is available.
