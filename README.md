### Paata Bugianishvili

20.07.2023

System OS: Windows 11

WebBrowser: Chrome. Version 115.0.5790.98 (Official Build) (64-bit))

# Task 1 - Exploratory Testing
1.	Enter all the required information in the registration form.
2.	Entering invalid information in the form, such as an incorrect email address or a phone number that is too long.
3.	Leaving some of the fields in the form blank.
4.	Check to make sure that I receive a confirmation message and an email after creating an account.
# Task 2 - Test Cases 
Test Case 1: user enters a valid email address and password. The account is created successfully, and a confirmation email is sent to the user's email address. (Test Case 1.01)

Test Case 2: user enters invalid information in the registration form, User should not be able to create account. (Test Case 1.02)

Test Case 3: user leaves some of the fields blank in registration form and should not be able to create account. (Test Case 1.03)

Test Case 4: user is trying to register without filling the required information, user should not be able to register. (Test Case 1.04)

Test Case 5: user tries fill all the information but using shorter password than required, user should not be able to create account. (Test Case 1.05)

# Task 3 - Test Run

### Test Case 1.01
Test Scenario: Enter all required information in the registration form.
Expected Result: user should be able to create an account successfully.

| Steps |  Data | Expected Result  |  Actual Result |
|---|---|---|---|
| Go to the Create a Free Account page  | https://cloud.test.yourbourse.com/free-account  |  Page will open with registration form |  Page is opening with. registration form |
| Enter Required information in the form  | Enter Valid Data  | Form will be filled |  Form is filled |
|  Captcha Checkbox  |  Check Captcha | Captcha will be checked  |  Captcha is Checked |
|  “Register” Button Click |  |  user should be redirected to a confirmation page | redirected to a confirmation page  |
|  Email Confirmation Check |  Checking filled email |  User should receive a confirmation email |  Confirmation email received. |

### Test Case 1.02
Test Scenario: Enter invalid information in the registration form.
Expected Result: user should not be able to create an account.

| Steps |  Data | Expected Result  |  Actual Result |
|---|---|---|---|
| Go to the Create a Free Account page  | https://cloud.test.yourbourse.com/free-account  |  Page will open with registration form |  Page is opening with. registration form |
| Enter Required information in the form  | Enter Invalid Data  | Form will be filled |  Form is filled |
|  Captcha Checkbox  |  Check Captcha | Captcha will be checked  |  Captcha is Checked |
|  “Register” Button Click |  | The user should see an error message | redirected to a confirmation page  |

### Test Case 1.03
Test Scenario: Leave some of the fields in the form blank.
Expected Result: The user should not be able to create an account.

| Steps |  Data | Expected Result  |  Actual Result |
|---|---|---|---|
| Go to the Create a Free Account page  | https://cloud.test.yourbourse.com/free-account  |  Page will open with registration form |  Page is opening with. registration form |
| Leave some fields in the registration form blank  | Leaving password and email blank  | Form will be filled without password and email |  Form is filled if filled without password and email |
|  Captcha Checkbox  |  Check Captcha | Captcha will be checked  |  Captcha is Checked |
|  “Register” Button Click |  | The user should see an error message |  Email and password fields gives us error to fill them also  |

### Test Case 1.04
Test Scenario: Trying to register without filling in the information.
Expected Result: The user should not be able to create an account.

| Steps |  Data | Expected Result  |  Actual Result |
|---|---|---|---|
| Go to the Create a Free Account page  | https://cloud.test.yourbourse.com/free-account  |  Page will open with registration form |  Page is opening with. registration form |
| Leave all the fields in the registration form blank | Not filling any information | Form will not be filled |  Form is not filled |
|  Captcha Checkbox  |  Check Captcha | Captcha will be checked  |  Captcha is Checked |
|  “Register” Button Click |  | The user should see an error message |  Getting error to fill data in fields  |

### Test Case 1.05
Test Scenario: Trying to register with short password.
Expected Result: The user should not be able to create an account.

| Steps |  Data | Expected Result  |  Actual Result |
|---|---|---|---|
| Go to the Create a Free Account page  | https://cloud.test.yourbourse.com/free-account  |  Page will open with registration form |  Page is opening with. registration form |
| Enter Required information with shorter password in the form | Using 5 characters max password | Form will be filled, error message will be displayed below password field |  Form is filled, error message is displayed below password field |
|  Captcha Checkbox  |  Check Captcha | Captcha will be checked  |  Captcha is Checked |
|  “Register” Button Click |  | The user can not register, and error message should be displayed below password field |  The user can not register, and error message is displayed below password field  |

Task 5 – User Experience 
My thoughts about registration form
1.	The form is well-organized and easy to follow. The fields are clearly labeled, and the instructions are clear.
2.	The error messages are clear and informative. They tell the user what went wrong and how to correct the error.
3.	The reCAPTCHA is a good way to prevent bots from creating accounts.
4.	The form is mobile friendly (I tried with chrome DevTools and it is responsive)

What  can be improved
1.	The form does not make validation of email so I can just type something@something without domain and it will still process to registration
2.	Also I can put symbols and numbers in names suchs as company name or surname or name
3.	Fields can have maximized characters for example I can type unlimited amount of characters in fields and that’s not good
4.	For phone you can make verification that enter phone number matches the country, (for now I can type whatever I want)
5.	Yes, I am getting confirmation on email but it will be better to make verification also, before user can log in to account he should make a verification from email that he got from the website with verification link.
6.	Registration could include progress bar for users to see how far along they are in the registration.
7.	could include a link to the privacy policy and terms of service.
8.	could be translated into other languages.
9.	could be made accessible to people with disabilities.
