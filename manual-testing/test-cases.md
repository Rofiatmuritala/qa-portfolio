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




## TC-LOGIN-002 — Unsuccessful Login With an Invalid Credentials

**Test ID:** TC-LOGIN-002

**Test Case:** Verify that login fails with an invalid username..

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

The user should be not be authenticated.

### Actual Result

The user was not authenticated

### Status

Pass



## TC-LOGIN-003 — Unsuccessful Login With Invalid Password

**Test ID:** TC-LOGIN-003

**Test Case:** Verify that login fails with an invalid password

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

The user should be not be authenticated.

### Actual Result

Username was not authenticated.

### Status

Pass




## TC-LOGIN-004 — Unsuccessful Login With Empty Username

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

The user should be not successfully authenticated.

### Actual Result

The user was not successfully authenticated.

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

The user should be not successfully authenticated.

### Actual Result

The user was not authenticated.

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

The user should be not successfully authenticated.

### Actual Result

The user was not authenticated.

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

The user should see an Invalid login error message

### Actual Result

Invalid login error message was displayed to the user.

### Status

pass




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
5. Redirected to the Products page.
6. Click on the Logout button.

### Expected Result

The user should be successfully logged out and redirected to the login page.

### Actual Result

The user should was successfully logged out and redirected to the login page.

### Status

Pass










