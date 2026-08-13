# SauceDemo — Test Cases

## TC-LOGIN-001 — Successful Login With Valid Credentials

**Test ID:** TC-LOGIN-001

**Test Case:** Verify that a user can log in with valid credentials.

**Module:** Login & Authentication

**Priority:** High

**Preconditions:**
- The SauceDemo login page is accessible.
- A valid test account is available.

**Test Data:**
- Valid username
- Valid password

### Test Steps

1. Open the SauceDemo login page.
2. Enter a valid username in the Username field.
3. Enter a valid password in the Password field.
4. Click the Login button.

### Expected Result

The user should be successfully authenticated and redirected to the Products page.

### Actual Result

The user was successfully authenticated and redirected to the Products page.

### Status

Pass




## TC-LOGIN-002 — Unsuccessful Login With an Invalid Username.

**Test ID:** TC-LOGIN-002

**Test Case:** Verify that login fails with an invalid username.

**Module:** Login & Authentication

**Priority:** High

**Preconditions:**
- The SauceDemo login page is accessible.
- A valid test account is available.

**Test Data:**
- Invalid username
- Valid password

### Test Steps

1. Open the SauceDemo login page.
2. Enter an invalid username in the Username field.
3. Enter a valid password in the Password field.
4. Click the Login button.

### Expected Result

The user should not be authenticated and should remain on the login page.

### Actual Result

The user was not authenticated and remained on the login page.

### Status

Pass



## TC-LOGIN-003 — Unsuccessful Login With Invalid Password.

**Test ID:** TC-LOGIN-003

**Test Case:** Verify that login fails with an invalid password.

**Module:** Login & Authentication

**Priority:** High

**Preconditions:**
- The SauceDemo login page is accessible.
- A valid test account is available.

**Test Data:**
- Valid username
- Invalid password

### Test Steps

1. Open the SauceDemo login page.
2. Enter a valid username in the Username field.
3. Enter an invalid password in the Password field.
4. Click the Login button.

### Expected Result

The user should not be authenticated and remain on the login page.

### Actual Result

The user was not authenticated and remained on the login page.

### Status

Pass




## TC-LOGIN-004 — Unsuccessful Login With Empty Username.

**Test ID:** TC-LOGIN-004

**Test Case:** Verify that login fails when the username is empty.

**Module:** Login & Authentication

**Priority:** High

**Preconditions:**
- The SauceDemo login page is accessible.
- A valid test account is available.

**Test Data:**
- Empty Username
- Valid Password

### Test Steps

1. Open the SauceDemo login page.
2. Leave the Username field empty.
3. Enter a valid password in the Password field.
4. Click the Login button.

### Expected Result

The system should prevent login and display a validation message indicating that the username is required.

### Actual Result

The system prevented login and displayed the message "Username is required."

### Status

Pass




## TC-LOGIN-005 — Unsuccessful Login With Empty Password

**Test ID:** TC-LOGIN-005

**Test Case:** Verify that login fails when the password is empty.

**Module:** Login & Authentication

**Priority:** High

**Preconditions:**
- The SauceDemo login page is accessible.
- A valid test account is available.

**Test Data:**
- Valid Username
- Empty Password

### Test Steps

1. Open the SauceDemo login page.
2. Enter a valid username in the Username field.
3. Leave the Password field empty.
4. Click the Login button.

### Expected Result

The system should prevent login and display a validation message indicating that the password is required.

### Actual Result

The system prevented login and displayed the message "Password is required."

### Status

Pass




## TC-LOGIN-006 — Unsuccessful Login With both Empty Username and Password

**Test ID:** TC-LOGIN-006

**Test Case:** Verify that login fails when both username and password are empty.

**Module:** Login & Authentication

**Priority:** High

**Preconditions:**
- The SauceDemo login page is accessible.
- A valid test account is available.

**Test Data:**
- Empty username
- Empty password

### Test Steps

1. Open the SauceDemo login page.
2. Leave the Username field empty.
3. Leave the Password field empty
4. Click the Login button.

### Expected Result

The system should prevent login and display a validation message indicating that the username is required.

### Actual Result

The system prevented login and displayed the message "Username is required."

### Status

Pass




## TC-LOGIN-007 — Unsuccessful Login With Invalid Credentials

**Test ID:** TC-LOGIN-007

**Test Case:** Verify that an appropriate error message is displayed for invalid login attempts.

**Module:** Login & Authentication

**Priority:** High

**Preconditions:**
- The SauceDemo login page is accessible.
- A valid test account is available.

**Test Data:**
- Invalid username
- Invalid password
  
### Test Steps

1. Open the SauceDemo login page.
2. Enter an invalid username in the Username field.
3. Enter an invalid password in the Password field.
4. Click the Login button.

### Expected Result

The system should prevent authentication and display the appropriate error message for invalid credentials.

### Actual Result

The system prevented authentication and displayed: "Username and password do not match any user in this service"

### Status

Pass




## TC-LOGIN-008 — Successful Logout 

**Test ID:** TC-LOGIN-008

**Test Case:** Verify that a logged-in user can log out successfully.

**Module:** Login & Authentication

**Priority:** High

**Preconditions:**
- The SauceDemo login page is accessible.
- A valid test account is available.

**Test Data:**
- Valid username
- Valid password

### Test Steps

1. Open the SauceDemo login page.
2. Enter a valid username in the Username field.
3. Enter a valid password in the Password field.
4. Click the Login button.
5. Verify that the user is redirected to the Products page.
6. Open the navigation menu.
7. Click the Logout button.

### Expected Result

The user should be logged out and redirected to the login page.

### Actual Result

The user was successfully logged out and redirected to the login page.

### Status

Pass










