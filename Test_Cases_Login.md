## Test Cases for Login functionality. 
---
This document contains a collection of manual test cases for a standard login functionality.

The test cases are designed to validate the most common login scenarios and demonstrate my approach to manual testing. They include both positive and negative test scenarios, covering input validation, authentication, and expected system behavior.

The purpose of these test cases is to showcase my ability to create clear, structured, and comprehensive test documentation following QA best practices.


## **ID: TC_001**

**Title:**  Verify login with valid credentials

**Priority:**
   High 

**Preconditions:**  User must be on the login page and User should exist. 

**Steps:**
1. Enter valid username
2. Enter valid password
3. Click on Login button

**Expected Result:**

User should be successfully logged in and redirected to the dashboard





## ID: TC_002

**Title:** 
Verify login with invalid password

**Priority:**
High

**Preconditions:**
User must be on the login page and user shouls exist. 

**Steps:**
1. Enter valid username
2. Enter incorrect password
3. Click on Login button

**Expected Result:**
Error message should be displayed: "Invalid username or password"


## ID: TC_003

**Title:**
Verify login with empty fields

**Priority:**
High 

**Preconditions:**
User must be on the login page

**Steps:**
1. Leave username field empty
2. Leave password field empty
3. Click on Login button

**Expected Result:**
Validation messages should appear for required fields



## ID: TC_004

**Title:**
Verify login with locked user account

**Priority:**
High

**Preconditions:**
User account must be locked

**Steps:**
1. Enter valid username of locked user
2. Enter valid password
3. Click on Login button

**Expected Result:**
User should not be able to login and should see account locked message




## ID: TC_005

**Title:**
Verify login using credentials in a different language

**Priority:**
Medium

**Preconditions:**
User must be on the login page and this user should not exist. 
Registered users are only in the English language. 

**Steps:**
1. Enter a username using non-Latin characters (e.g., Georgian: `მარიამი`).
2. Enter a password using non-Latin characters (e.g., `პაროლი123`).
3. Click the **Login** button.

**Expected Result:**
The system should handle the input correctly. If non-Latin characters are not supported, an appropriate validation or error message should be displayed, and the user should not be logged in.






