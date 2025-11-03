The Purchase Request Management System is a digital solution built using Microsoft Power Platform tools to automate and streamline the purchase request (PR) process within an organization.
It allows users to create, track, and approve purchase requests through a Canvas App, supported by Power Automate workflows and an AI-powered Copilot chatbot for quick access and updates.

System Components
1. Canvas App (Power Apps)

User-friendly interface for submitting and tracking purchase requests.

Connects to a SharePoint List or Dataverse table storing all PR details.

Supports form validation, file attachments (e.g., quotations), and conditional approval routing.

Allows department-based views (e.g., see “My Department’s PRs”).

Main Screens:

Home / Dashboard: Overview of requests with edit and delete and show details buttons.

New Request: Form for submitting a new purchase request.

My Requests: Shows the user’s requests and their statuses.

Approvals: Displays PRs awaiting approval (for managers).



2. Power Automate Flows

Automated workflows that handle the process logic, notifications, and approvals.

Key Flows:

New PR Submission Flow

Triggered when a new record is created.

Sends a notification or approval request to the manager.

Approval Decision Flow

Handles manager approval/rejection.

Updates PR status automatically in the data source.

Sends email notifications to the requester.





Copilot Chatbot (Power Virtual Agents / Copilot Studio)

An intelligent conversational assistant embedded in Teams or the Canvas App.

Capabilities:

Responds to user questions like:

“Show my pending PRs”

“Get PR details by ID”

“List PRs from the IT department”



Data Source:Microsoft Dataverse





How It Works 

User Submits Request

Data saved in Dataverse.

Power Automate triggers workflow.

Manager Receives Approval Request

Email or Teams notification with Approve/Reject options.

Request Status Updated Automatically

The flow updates the record and notifies the requester.

Chatbot Access

User asks Copilot for request updates.

Bot fetches data using dataverse