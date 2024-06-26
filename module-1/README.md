
| Product Name | Product Version | Module Name | Feature Name | Update Date | Updated By
|---|---|---|---|---|---|
| eBiocore | 1.0 | Delete | Customer Bio Metric Delete (Finger Delete) | 26/06/2024 | Aysa Siddika

***

# Objective
If the customer finger is enrolled in new system then as per request of customer and back office user system will delete finger from biocore system usion delete API.

# Operations
Click delete button and confirm if you want to delete finger, after clicking OK delete API will be called and delete the finger from new system.

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
| Verify | API | POST | Verify the customer in new system with online matching
| f106_page_83.sql | Apex Page | Capture Finger | Show the biocore widget to capture finger of customer to verify
|f107_page_268.sql|Apex Page | Customer Creation | Customer point information getting
# Dependencies
Finger device drivers and ERA Biocore exe file.
