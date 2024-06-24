
| Product Name | Product Version | Module Name | Feature Name | Update Date | Updated By
|---|---|---|---|---|---|
| eBiocore | 1.0 | Verify | Customer Registration (Finger Verify) | 24/06/2024 | Aysa Siddika

***

# Objective
If the customer point is setup to capture customer finger with new Biocore system then new widget will apear in customer finger verification after enrollment.

# Operations
Click verify button and new widget of Biocore will apear where customer finger is mandatory, after capturing one finger and meet score 80 then system will automatically call verify API to verify the finger of the customer with iso template in new finger system which was enrolled earlier.

### Step -1
Click Verify Button
![Click Enroll Button](images/Verify1.png)
### Step-2
Capture Finger To verify

![Capture Finger](images/Verify2.png)
### Step-3
After successfully verifying customer finger
![After successfully enrolling customer finger](images/Verify3.png)


| Resource Name | Resource Type | Operation | Remarks | 
|---|---|---|---|
| TOKEN | API | GET | Get Access Token to call Verify API
| Verify | API | POST | Verify the customer in new system with online matching
| f106_page_83.sql | Apex Page | Capture Finger | Show the biocore widget to capture finger of customer to verify
| f106_page_84.sql | Apex Page | Capture Finger | Show the old system to capture finger of customer to verify
|f107_page_500.sql|Apex Page | Customer Creation | Customer point information getting
|f107_page_504.sql|Apex Page | Capture Customer Photo | Customer point information getting
|f107_page_505.sql|Apex Page | Finger Verify | Customer point information getting and new or old finger Verify made available according to setup. 
# Dependencies
Finger device drivers and ERA Biocore exe file.

