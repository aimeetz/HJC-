# Registration Page
## List of Registration Page requirements:

Required fields are:
1. User name
1. Password
1. Confirm Password
1. Phone number
1. Captcha

Validation for fields:
1. Username: It should have alphanumeric, Length should be 3 to 10 (for F6 website), 5-8 (for H6 website)
1. Password: It should have alphanumeric, Length should be 6 to 18
1. Phone number: Phone number should have only numbers, Chinese phone number is required, length should be 11 digits

## Test cases for Registration Page
|Test cases|Feature|Description|Step to Execute|Test Data|Expected results|
|---|---|---|---|:---:|---|
|1|Required fields|Check the required fields by not filling any data|1. Do not enter any value in the field ́2. Click on the Register button|N/A|It should show validation message and user should not registered successfully|
|2|Required fields|Check user should Register by filling all the required fields|1. Enter valid values in the required fields 2. Click the Register button|N/A|1. Users should be registered successfully. 2. It should jump into Personal information Page|
|3|Phone Number validation|Check the phone number when passing alphanumeric data|1. Enter alphanumeric data in phone field 2. Click on Register button|abc21680005 |It should show the validation error message for phone number format|
|4|Phone Number validation|Check the phone number when passing valid number|1. Enter valid phone number 2.Click on Register button|16521680005|It should not show any validation message|
|5|Phone Number validation|Verify if the length of the phone number is incorrect less than 11|1. Enter phone number less than 11 digits. 2.Enter all required fields 3.Click on Register Button|1652168000|It should show the validation error message for phone number format|
|6|Phone Number validation|Verify if the length of the phone number is incorrect more than 11|1. Enter phone number less than 11 digits 2.Enter all required fields 3.Click on Register Button|1652168000555|It should show the validation error message for phone number format|
|7|Username validation|Check the username limit when enter value less than min or enter value more than max|1. Enter value which is alphanumeric but less than 3 or more than 10 2.Click on Registration button|Any Random string with numbers|It should show proper error message|
|8|Password validation|Check the password limit when enter value less than min or enter value more than max|1. Enter value which is alphanumeric but less than 6 or more than 18 2.Click on Registration button|Any Random string with numbers|It should show proper error message|
|9|Password Validation|Verify user should get an error message when password and confirm password not matches|1. Enter valid values in the required fields. 2. Enter a password 3. Enter a different confirm password 4. Click on the Registration button|N/A|Users should get an error message that password and confirm password not matches|
|10|Required Fields|Verify if blank spaces are passed in required fields.|1. Go to the Site. 2. Passed blank spaces in required fields. 3. Click on the Register button|N/A|Validation error message for required fields should visible|

# Login Page

## Login page requirements, such as:
- Username, password and captcha are mandatory fields 
- The limit of the Username should be 3-10 characters (alphanumeric). The limit of the Password should be 6-18 characters (alphanumeric).

## Test cases for log in page

|Test cases|Feature|Description|Step to Execute|Expected results|
|---|---|---|---|---|
|1|Required Fields|Check the required fields by not filling any data|1. Not filling any data on required fields 2. Click on Login button| User should not login and should show proper error message: login account is a required value|
|2|User Login|Check when passing a correct username and invalid password|1. Enter valid username 2. Enter incorrect password 3. Enter correct captcha 4. Click on Login Button|User should not log in and should show proper error message|
|3|User Login|Verify when passing incorrect username and correct password|1. Enter incorrect username 2. Enter the correct password and captcha 3. Click on the Login Button|User should not be able to log in and the error message should be displayed|
|4|User Login|Verify when passing correct username, correct password and incorrect captcha| 1. Enter valid username and correct password 2. Enter incorrect captcha 3. Click on the Login Button| User should not log in and should show proper error message|
|5|User Interface|Check Keeping Password|1. Enter valid username 2. Do not enter password 3. Enter correct captcha 4. Click on Login Button|User should not log in and should show proper error message|
|6|User Login|Check when pass correct username, password and captcha|1. Enter valid username 2. Enter valid password 3. Enter valid captcha 4.Click on Login Button| User should log in and jump to home page|
|7|User Login|Verify when passing incorrect username, password, captcha| 1. Enter incorrect username 2. Enter the incorrect password 3.Enter incorrect captcha 4. Click on the Login Button|User should not be able to log in and the error message should be displayed|
|8|Required Fields|Verify if blank spaces are passed in required fields|1. Passed blank spaces in required fields 2. Click on the Login button|Those Blank spaces should trim and Validation error message for required fields should visible|
|9|Password Validation|Check the password limit when enter value less than min or enter value more than max|1. Enter value which is alphanumeric but less than 6 or more than 18 2.Click on Login button|It should show proper error message|
|10|Username Validation|Check the username limit when enter value less than min or enter value more than max|1. Enter value which is alphanumeric but less than 3 or more than 10 2.Click on Login button|It should show proper error message|

