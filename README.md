Welcome to the 4Fresh Human Resource Application! This application was developed as part of the Google Workspace Hackathon 2024 organized by APU. 
Our team chose the Human Resource case study, focusing on Automated Leave Tracking and Management.

Our solution provides two main automations/extensions to streamline HR processes:
a) Leave Tracking Generator
b) Calendar Employee Leave & Leave Email Reminder

Before starting on trying to use our application, please access the two links that are provided below:
1) Link for accessing the Google Sheet that was created by our team. All the data of our application will be stored in this google sheet.
   https://docs.google.com/spreadsheets/d/104_3JVpb_1V6EgvwoKxnfXQ7y0Q3dL4QHaWgxdWKn-c/edit?usp=sharing

   Note: ANYONE WITH THE LINK CAN EDIT THE SHEETS.
   
3) Link for accessing the Google Forms that are used to collect/gather the leave request data from employees
   https://docs.google.com/forms/d/e/1FAIpQLSdOtccB0FmLtvciCdkljSBusitW9djdML3Y7RsMMJNnDKFsXA/viewform


Viewing the App Script Code
To view our App Script code:
1. Visit the Google Sheets link below.
   https://docs.google.com/spreadsheets/d/104_3JVpb_1V6EgvwoKxnfXQ7y0Q3dL4QHaWgxdWKn-c/edit?usp=sharing
2. Go to the Extensions tab and click on Apps Script.
   ![image](https://github.com/user-attachments/assets/6c9698e7-dca5-4176-bcb9-1c80272a86a4)
3. You will find our source code in the Editor tab.
4. FYI, we have created 6 triggers to ensure smooth operation of our automations. You may find them in the 'Triggers' tab of Apps Script.
   ![image](https://github.com/user-attachments/assets/0f501fba-c7a2-447b-95ae-482b489013a6)

Note: Or you may also view the source code that we uploaded for submission on this GitHub.

User Manual for Automation 1: Leave Tracking Generator
Before You Begin:
1. Set Employee Email:
   -Go to the EmployeeResponses sheet in the spreadsheet.
   -Change one of the existing employee email addresses to your own to receive email notifications.

3. Set Manager Email:
   -Go to the Manager sheet in the spreadsheet.
   -Change one of the manager email addresses to another email address you own.
   -Ensure you set the manager responsible for the department the employee belongs to. For example, if you change an employee's email, note their Department ID, find it in the Department table,
    retrieve the corresponding ManagerID, and set the correct manager email.

   Note: You need two different email addresses to receive notifications: one for employees and one for managers.

Steps to Use the Leave Tracking Generator:
1. Apply for Leave:
   Visit the Google Forms link to submit your leave application.
   Link: https://docs.google.com/forms/d/e/1FAIpQLSdOtccB0FmLtvciCdkljSBusitW9djdML3Y7RsMMJNnDKFsXA/viewform

3. Check Leave Balance:
   -Before applying for leave, you can check your leave balance via the link
    https://www.appsheet.com/start/315af32e-45da-4cb7-9ebc-8f3dafe54467?platform=desktop#viewStack[0][identifier][Type]=Control&viewStack[0][identifier][Name]=Employee%20Records&appName=4FreshHumanResource-854965436-24-07-12
   -Login using the employee email address you changed in the EmployeeResponses sheet. You can only view your own leave balance.

4. Receive Notifications:
   -After submitting the form, you will receive an email with the subject:
      -"Leave Request Submitted" (if requested duration ≤ Leave balance)
      -"Insufficient Leave Balance" (if requested duration > Leave balance)
   -The responsible manager will also receive a notification email with the subject "New Leave Request Submitted by...", which includes a link to our app to review the request.

   Note:
   -HR managers can view and review all leave requests.
   -Department managers can only view and review requests for their own department.
   -Emails not listed in the Manager table cannot view or review leave requests.

5. Approval Process:
   -When the manager approves or rejects a leave request through the app, the leave balance is automatically updated for the employee.
   -An email notification is sent to the employee confirming the approval or rejection.

That's the end of Automation 1. There is no additional action needed in the spreadsheet. The Google Sheets document is only used for data storage for Automation 1.
