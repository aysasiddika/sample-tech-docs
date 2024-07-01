
| Product Name | Product Version | Module Name | Feature Name | Update Date | Updated By
|---|---|---|---|---|---|
| eBiocore | 1.0 | Delete | Customer Bio Metric Migration | 01/07/2024 | Aysa Siddika

***

# Objective
Old system customer finger data migrate to new system after verification with OTP & old finger.
# Operations
Click verify button and give finger of customer. After verification of finger new enroll widget will open. Customer will give finger again and after second time verification OTP will be sent to Customer and after giving OTP customer finger will be enrolled in new system.

### Step -1
Go to system module and under configuration click on Cancel Bio Metric Enrollment Menu.

![Click Enroll Button](images/Delete1.png)
### Step-2
Select specific customer or agent then click delete button and confirm by clicking ok to delete the finger.

![Capture Finger](images/Delete2.png)
### Step-3
After successfully calling delete API finger deletion successful.

![After successfully enrolling customer finger](images/Delete3.png)


| Resource Name | Resource Type | Operation | Remarks | 
|---|---|---|---|
| TOKEN | API | GET | Get Access Token to call Verify API
| DELETE | API | POST | Delete finger in new system
| f106_page_143.sql | Apex Page | Delete Finger | Delete finger from new and old system.
|EMOB.CALL_BIOCORE_API | Package | Finger Delete API | Delete finger from new system

# Dependencies
Finger device drivers and ERA Biocore exe file.
