# IPC Database Issue Tracker

This tool is a centralised tracker of change requests and defect (bug) reports for all SDMS-like applications 
developed by the International Paralympic Committee (IPC). Consequently, only the licence holder of the relevant 
application, in this case the IBSA federation, has access to that section.

## Change Requests<!-- {docsify-ignore} -->

A change request is the desire to change, adapt or extend the current functionality of the tool that has not been 
included in the initially launched version. Each change request belongs to one of the following categories:
- New feature: Anything related to a complete new functionality request to get rid of otherwise manual or 
  paper-related handling of data.
- Business process: Required adjustment of the tool according to recently implemented changes in the business 
  processes of the NPC or NF.
- User experience: Related to the user-friendliness of the tool to enhance the quality of reports, handling of 
  data inside the system, or the look&feel of the application.
- Rule change: When sport and classification rules change, it is often required that the software developed based 
  on the previous rules must change likewise to cover again the new rules and regulations of a sport or the Paralympic movement.

When registering a new change request, following fields appear:

| **Field**                                                        | **Format** | **Comments**                                                                                                         |
| ---------------------------------------------------------------- | ---------- | -------------------------------------------------------------------------------------------------------------------- |
| **Application**                                                  | ISAS      |                                                                                                                      |
| **Requestor**                                                    | text (50)  | Automatically populated with the username of the person who is about to submit the request.                          |
| **Request Time Stamp**                                           | datetime   | Automatically populated with the timestamp when the change request has been submitted.                               |
| **Priority**                                                     | dropdown   | How important is the change request? (low, medium, high)                                                             |
| **Severity**                                                     | dropdown   | <span class="asterisk">1</span>                                                                                      |
| **Category**                                                     | dropdown   | To which change request category does the request belongs to (see list above for details)                            |
| **Title**                                                        | text (100) | Short (!) descriptive title what the change request is about                                                         |
| **Description**                                                  | text       | <span class="asterisk">2</span>                                                                                      |
| **Requested Completion**                                         | date       | Date by when the completion of the change request is optimal?                                                        |
| **Attachment**                                                   | file       | Any supporting file (rule book, template, screenshots, drawings, images) can be attached here as supporting material |
| <span class="table-header">Feedback by IPC Sports IT team</span> |            |                                                                                                                      |
| **Request Status**                                               | dropdown   | <span class="asterisk">3</span>                                                                                      |
| **Responsible Developer**                                        | text (50)  | Username of the IPC Sports IT Team staff member that is in charge of the change request.                             |
| **Estimated Delivery Date**                                      | date       |                                                                                                                      |
| **Estimated Working Time**                                       | float      | Number of hours that the team will likely spend on the implementation of the change.                                 |
| **Developers Feedback**                                          | text       | The Sports IT team will provide further information and feedback in here.                                            |


<span class="asterisk">1. </span>How severe is the change request, how much are the current business processes affected/slowed down unless the request is accepted and realised? (low, medium, high)

<span class="asterisk">2. </span>Text area to describe now the details: 
  - Which module(s) and tables of the applications are affected?
  - What is the underlying business process?
  - What are potential further impacts?

<span class="asterisk">3. </span>Reflects the current process status of the change request. The NPC can only amend a change request if status is New or Imprecise. Rejected or Cancelled change requests will not be further handled.

The IPC Sports IT team will be automatically informed about the registration of any new change request by email. 
The IPC will come back to the NPC to discuss the impact of the change request or clarify further questions if necessary.

In any case, the responsible developer will change the request status and populate further information. The requestor 
is then automatically informed about any change in the request status or delivery date by email but can also go into 
ISAS and check the information online.