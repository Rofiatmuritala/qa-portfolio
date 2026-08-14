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



## TC-LOGIN-008 — Successful Login Redirects to Products Page

**Test ID:** TC-LOGIN-008

**Test Case:** Verify that a user is redirected to the Products page after successfully logging in.

**Module:** Login & Authentication

**Priority:** High

**Preconditions:**

- The SauceDemo login page is accessible.
- A valid test account is available.

**Test Data:**

- Username: 'performance_glitch_user'
- Valid password

### Test Steps

1. Open the SauceDemo login page.
2. Enter the username 'performance_glitch_user'.
3. Enter the valid password.
4. Click the Login button.
5. Observe the page displayed after authentication.

### Expected Result

The user should be successfully authenticated and redirected to the Products page.

### Actual Result

The user was successfully authenticated, but instead of being redirected to the Products page, the application redirected the user to a Product Details page.

### Status

Fail



## TC-LOGIN-009 — Locked-Out User Cannot Log In

**Test ID:** TC-LOGIN-009

**Test Case:** Verify that a locked-out user can not log in.

**Module:** Login & Authentication

**Priority:** High

**Preconditions:**

- The SauceDemo login page is accessible.
- A locked-out test account is available.

**Test Data:**

- Username: 'locked_out_user'
- Valid password

### Test Steps

1. Open the SauceDemo login page.
2. Enter 'locked_out_user' in the Username field.
3. Enter the valid password.
4. Click the Login button.
5. Observe the response.

### Expected Result

The system should prevent the locked-out user from logging in and display an appropriate validation message.

### Actual Result

The system prevented the user from logging in and displayed the message:

> "Sorry, this user has been locked out."

### Status

Pass


## TC-LOGIN-010 — Successful Logout 

**Test ID:** TC-LOGIN-010

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




## TC-PRODUCT-001 — Products Page Displays Available Products

**Test ID:** TC-PRODUCT-001

**Test Case:** Verify that the Products page displays available products.

**Module:** Product Browsing & Product Details

**Priority:** High

**Preconditions:**
- User is logged in successfully.
- User is on the Products page.

**Test Data:**
- Not applicable

### Test Steps

1. Log in with valid credentials.
2. Navigate to the Products page.
3. Observe the product listing.

### Expected Result

The Products page should display the available products correctly.

### Actual Result

The Products page displayed the available products correctly.

### Status

Pass


## TC-PRODUCT-002 — Product Cards Display Correct Information

**Test ID:** TC-PRODUCT-002

**Test Case:** Verify that each product displays the correct name, price, description, and image.

**Module:** Product Browsing & Product Details

**Priority:** High

**Preconditions:**
- User is logged in successfully.
- User is on the Products page.

**Test Data:**
- Not applicable

### Test Steps

1. Log in with valid credentials.
2. Navigate to the Products page.
3. Select a product.
4. Verify that the product name is displayed.
5. Verify that the product description is displayed.
6. Verify that the product price is displayed.
7. Verify that the product image is displayed.

### Expected Result

Each product should display its corresponding name, description, price, and image.

### Actual Result

Each product displayed its corresponding name, description, price, and image.

### Status

Pass


## TC-PRODUCT-003 — Open Product Details

**Test ID:** TC-PRODUCT-003

**Test Case:** Verify that a user can open a product's details.

**Module:** Product Browsing & Product Details

**Priority:** High

**Preconditions:**
- User is logged in successfully.
- User is on the Products page.
- At least one product is available.

**Test Data:**
- Not applicable

### Test Steps

1. Log in with valid credentials.
2. Navigate to the Products page.
3. Select a product by clicking its image or name.

### Expected Result

The selected product's details page should open successfully.

### Actual Result

The selected product's details page was opened successfully.

### Status

Pass


## TC-PRODUCT-004— Product Details Contain Correct Information

**Test ID:** TC-PRODUCT-004

**Test Case:** Verify that the product details contain the correct product information.

**Module:** Product Browsing & Product Details

**Priority:** High

**Preconditions:**
- User is logged in successfully.
- User is on the Products page.
- At least one product is available.

**Test Data:**
- Username: 'problem_user'
- Product: Sauce Labs Backpack

### Test Steps

1. Log in with valid credentials.
2. Navigate to the Products page.
3. Select a product.
4. Note the product name, price, description, and image displayed on the Products page.
5. Open the product details page.
6. Compare the product name, price, description, and image with the information previously observed.


### Expected Result

The product details page should display the same product name, price, description, and image as the corresponding product on the Products page.


### Actual Result

The Product details do not contain the correct product information with the ones on the product page.

### Actual Result

Fail



## TC-PRODUCT-005 — Return to Products From Product Details

**Test ID:** TC-PRODUCT-005

**Test Case:** Verify that a user can return from the product details page to the Products page.

**Module:** Product Browsing & Product Details

**Priority:** High

**Preconditions:**
- User is logged in successfully.
- User is on the Products page.

**Test Data:**
- Not applicable

### Test Steps

1. Log in with valid credentials.
2. Navigate to the Products page.
3. Select a product.
4. Verify that the product details page opens.
5. Click "Back to Products."

### Expected Result

The user should be returned to the Products page.

### Actual Result

The user was successfully returned to the Products page by clicking "Back to Products."

### Status

Pass


## TC-PRODUCT-006 — Product Sorting

**Test ID:** TC-PRODUCT-006

**Test Case:** Verify that products can be sorted according to the available sorting options.

**Module:** Product Browsing & Product Details

**Priority:** High

**Preconditions:**
- User is logged in successfully.
- User is on the Products page.

**Test Data:**
- Username: 'error_user'
- Username: 'problem_user'
- Sorting options: Available sorting options on the Products page

### Test Steps

1. The SauceDemo application is accessible.
2. A valid test account is available.
3. User is logged in successfully.
4. Navigate to the Products page.
5. Open the product sorting dropdown.
6. Select one of the available sorting options.
7. Observe the product list.
8. Verify that the products are displayed according to the selected sorting option.

### Expected Result

Products should be rearranged according to the selected sorting option without displaying an error.

### Actual Result

### Actual Result

- With 'error_user', the sorting functionality did not work, the application displayed the error message: "Sorting is broken! This error has been reported to Backtrace."
- With 'problem_user', the sorting functionality did not work, but no error message was displayed.
  
### Status

Fail




## TC-PRODUCT-006 — Product Sorting

**Test ID:** TC-PRODUCT-006

**Test Case:** Verify that products can be sorted according to the available sorting options.

**Module:** Product Browsing & Product Details

**Priority:** High

**Preconditions:**
- User is logged in successfully.
- User is on the Products page.

**Test Data:**
- Username: 'error_user'
- Username: 'problem_user'
- Sorting options: Available sorting options on the Products page

### Test Steps

1. The SauceDemo application is accessible.
2. A valid test account is available.
3. User is logged in successfully.
4. Navigate to the Products page.
5. Open the product sorting dropdown.
6. Select one of the available sorting options.
7. Observe the product list.
8. Verify that the products are displayed according to the selected sorting option.

### Expected Result

Products should be rearranged according to the selected sorting option without displaying an error.

### Actual Result

### Actual Result

- With 'error_user', the sorting functionality did not work, the application displayed the error message: "Sorting is broken! This error has been reported to Backtrace."
- With 'problem_user', the sorting functionality did not work, but no error message was displayed.
  
### Status

Fail




## TC-CART-001— Add One Product to Cart

**Test ID:** TC-CART-001

**Test Case:** Verify that a user can add a product to the cart.

**Module:** Cart

**Priority:** High

**Preconditions:**
- User is logged in successfully.
- User is on the Products page.
- At least one product is available

**Test Data:**
- Product: Sauce Labs Backpack
- Price: $29.99

### Test Steps

1. Navigate to the Products page.
2. Locate the selected product.
3. Click the **Add to cart** button.
4. Open the shopping cart.
5. Verify that the selected product is displayed in the cart.

### Expected Result

The selected product should be added to the shopping cart and displayed with the correct product name and price.

### Actual Result

The Sauce Labs Backpack was successfully added to the shopping cart and displayed with the correct name and price of $29.99.
  
### Status

Pass


## TC-CART-002 — Add Multiple Products to Cart

**Test ID:** TC-CART-002

**Test Case:** Verify that a user can add multiple products to the cart.

**Module:** Shopping Cart

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- User is on the Products page.
- At least two products are available.

**Test Data:**

- Product 1: Sauce Labs Backpack
- Price: $29.99
- Product 2: Sauce Labs Onesie
- Price: $7.99

### Test Steps

1. Navigate to the Products page.
2. Locate the Sauce Labs Backpack.
3. Click **Add to cart**.
4. Locate the Sauce Labs Onesie.
5. Click **Add to cart**.
6. Open the shopping cart.
7. Verify that both products are displayed.

### Expected Result

Both selected products should be added to the shopping cart. The cart count should reflect the number of items added, and both products should be displayed with their correct names and prices.


### Actual Result

Both selected products were successfully added to the shopping cart. The cart count reflected the number of items added, and both products were displayed with their correct names and prices.

### Status

Pass









