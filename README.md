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
4. FYI, we have created 5 triggers to ensure smooth operation of our automations. You may find them in the 'Triggers' tab of Apps Script.
   
   ![image](https://github.com/user-attachments/assets/4e10ebf1-bbf4-4837-81d6-b4cbadac3def)


Note: Or you may also view the source code that we uploaded for submission on this GitHub.




User Manual for Automation 1: Leave Tracking Generator
Before You Begin:
1. Set Employee Email:


   -Go to the EmployeeResponses sheet in the spreadsheet.

   -Change one of the existing employee email addresses to your own to receive email notifications.

2. Set Manager Email:
   
   -Go to the Manager sheet in the spreadsheet.
   
   -Change one of the manager email addresses to another email address you own.
   
   -Ensure you set the manager responsible for the department the employee belongs to. For example, if you change an employee's email, note their Department ID, find it in the Department table,
    retrieve the corresponding ManagerID, and set the correct manager email.
   

   Note: You need two different email addresses to receive notifications: one for employees and one for managers.

Steps to Use the Leave Tracking Generator:
1. Apply for Leave:
   
   Visit the Google Forms link to submit your leave application.
   
   Link: https://docs.google.com/forms/d/e/1FAIpQLSdOtccB0FmLtvciCdkljSBusitW9djdML3Y7RsMMJNnDKFsXA/viewform

2. Check Leave Balance:
   
   -Before applying for leave, you can check your leave balance via the link
    https://www.appsheet.com/start/315af32e-45da-4cb7-9ebc-8f3dafe54467?platform=desktop#vss=H4sIAAAAAAAAA62PvQoCMRCEX0WmzhOkFQsRLVRsjEW87EEwlxyXnHqEvLt7_iBYquXO8H3MZpwtXTZJVyfIfX5fCxogkRW2Q0sKUmEafOqCUxAKK908wlnTujAQTdZUhc5EhYJyEC9PogiZv9PI_6wRsIZ8srWlbnSOBnY9ea5HmoNPFkWg6ZM-Oro_wmwpnNWh6iOZHU_7YVKc-9m11d4sg2F1rV2kcgOiwCM5jQEAAA==&view=Employee%20Records&appName=4FreshHumanResource-854965436-24-07-12
   
   -Login using the employee email address you changed in the EmployeeResponses sheet. You can only view your own leave balance.

3. Receive Notifications:
   
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


User Manual for Automation 2: Calendar Employee Leave & Leave Email Reminder

Syncing Approved Leave
1. Approve a Leave Request:
   
-Open the app and navigate to the pending leave requests.

-Select a leave request and click "Approve."


2. Check the Department Leave Calendar:
   
-Switch to the department leave calendar view.

-The approved leave request will be automatically added to the calendar and marked on the respective dates.


3. Manager Access:
   
-Only managers are able to view their own department leave.

-Leave requests are categorized according to leave type, with different leave types shown in different colors.

-By clicking the bar, details of the leave will be shown in read-only mode.


Email Notifications

1. Automatic Email Notifications:
   
-The system will send an email notification to the employee one day before their leave starts and one day before their leave ends.


That's the end of Automation 2. 

Thanks for viewing!!!
