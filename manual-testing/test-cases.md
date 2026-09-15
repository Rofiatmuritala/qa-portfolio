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



## TC-CART-001 — Add One Product to Cart

**Test ID:** TC-CART-001

**Test Case:** Verify that a user can add a product to the cart.

**Module:** Shopping Cart

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- User is on the Products page.
- At least one product is available.

**Test Data:**

- Product: Sauce Labs Backpack
- Price: $29.99

### Test Steps

1. Navigate to the Products page.
2. Locate the Sauce Labs Backpack.
3. Click the **Add to cart** button.
4. Open the shopping cart.
5. Verify that the Sauce Labs Backpack is displayed in the cart.

### Expected Result

The selected product should be added to the shopping cart and displayed with the correct product name and price.

### Actual Result

The Sauce Labs Backpack was successfully added to the shopping cart and displayed with the correct product name and price of $29.99.

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
2. Locate the fSauce Labs Backpack.
3. Click **Add to cart**.
4. Locate the Sauce Labs Onesie.
5. Click **Add to cart**.
6. Verify that the cart count reflects the number of items added.
7. Open the shopping cart.
8. Verify that both products are displayed.

### Expected Result

Both selected products should be added to the shopping cart. The cart count should reflect the number of items added, and both products should be displayed with their correct names and prices.


### Actual Result

Both selected products were successfully added to the shopping cart. The cart count reflected the number of items added, and both products were displayed with their correct names and prices.


### Status

Pass



## TC-CART-003 — Cart Count Updates After Adding Products

**Test ID:** TC-CART-003

**Test Case:** Verify that the cart count updates correctly after adding products.

**Module:** Shopping Cart

**Priority:** Medium

**Preconditions:**

- User is logged in successfully.
- User is on the Products page.
- The shopping cart is empty.

**Test Data:**

- Product 1: Sauce Labs Backpack
- Product 2: Sauce Labs Onesie

### Test Steps

1. Navigate to the Products page.
2. Verify that the shopping cart does not display an item count.
3. Add the Sauce Labs Backpack to the cart.
4. Observe the cart count.
5. Add the Sauce Labs Onesie to the cart.
6. Observe the cart count again.

### Expected Result

The cart count should update correctly after each product is added. The count should reflect the total number of products added to the cart.

### Actual Result

The cart count updated correctly after each product was added and reflected the total number of products in the cart.

### Status

Pass


## TC-CART-004 — Added Product Displays Correct Information

**Test ID:** TC-CART-004

**Test Case:** Verify that the selected product appears in the cart with the correct information.

**Module:** Shopping Cart

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- User is on the Products page.
- At least one product is available.

**Test Data:**

- Product: Sauce Labs Backpack
- Price: $29.99

### Test Steps

1. Navigate to the Products page.
2. Locate the Sauce Labs Backpack.
3. Note the product name and price.
4. Click **Add to cart**.
5. Open the shopping cart.
6. Compare the product information in the cart with the information displayed on the Products page.

### Expected Result

The product displayed in the cart should have the same product name and price as the product selected on the Products page.

### Actual Result

The Sauce Labs Backpack displayed in the cart had the same product name and price of $29.99 as shown on the Products page.

### Status

Pass


## TC-CART-005 — Remove Product From Cart

**Test ID:** TC-CART-005

**Test Case:** Verify that a user can remove a selected product from the cart.

**Module:** Shopping Cart

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- At least two products have been added to the cart.
- User is viewing the shopping cart.

**Test Data:**

- Product 1: Sauce Labs Backpack
- Product 2: Sauce Labs Onesie

### Test Steps

1. Open the shopping cart containing at least two products.
2. Select the **Remove** button for one product.
3. Observe the products remaining in the cart.
4. Observe the cart count.

### Expected Result

The selected product should be removed from the cart. The remaining product should stay in the cart, and the cart count should decrease accordingly.

### Actual Result

The selected product was removed successfully. The remaining product stayed in the cart, and the cart count decreased from 2 to 1.

### Status

Pass



## TC-CART-006 — Cart Count Updates After Removing Products

**Test ID:** TC-CART-006

**Test Case:** Verify that the cart count updates correctly after removing products.

**Module:** Shopping Cart

**Priority:** Medium

**Preconditions:**

- User is logged in successfully.
- User is on the Products page.
- The shopping cart is empty.

**Test Data:**

- Product 1: Sauce Labs Backpack
- Product 2: Sauce Labs Onesie

### Test Steps

1. Navigate to the Products page.
2. Add the Sauce Labs Backpack to the cart.
3. Verify that the cart count is 1.
4. Add the Sauce Labs Onesie to the cart.
5. Verify that the cart count is 2.
6. Open the shopping cart.
7. Remove one product.
8. Verify that the cart count decreases to 1.
9. Remove the remaining product.
10. Observe the shopping cart.

### Expected Result

The cart count should decrease accordingly whenever a product is removed. After all products are removed, the cart should be empty and the item count should no longer be displayed.

### Actual Result

The cart count decreased from 2 to 1 after one product was removed. After the remaining product was removed, the cart became empty and the item count was no longer displayed.

### Status

Pass



## TC-CART-007 — Continue Shopping From Cart

**Test ID:** TC-CART-007

**Test Case:** Verify that a user can continue shopping from the cart without losing the products already added.

**Module:** Shopping Cart

**Priority:** Medium

**Preconditions:**

- User is logged in successfully.
- At least one product has been added to the cart.
- User is viewing the shopping cart.

**Test Data:**

- Product: Sauce Labs Backpack
- Price: $29.99

### Test Steps

1. Add the Sauce Labs Backpack to the cart.
2. Open the shopping cart.
3. Click **Continue Shopping**.
4. Verify that the user is returned to the Products page.
5. Open the shopping cart again.
6. Verify that the previously added product is still displayed.

### Expected Result

The user should be returned to the Products page, and the product previously added to the cart should remain unchanged.

### Actual Result

The user was returned to the Products page, and the previously added product remained unchanged in the cart.

### Status

Pass



## TC-CART-008 — Cart Displays Correct Product Information and Price

**Test ID:** TC-CART-008

**Test Case:** Verify that the cart displays the correct product information and price.

**Module:** Shopping Cart

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- User is on the Products page.
- At least one product is available.

**Test Data:**

- Product: Sauce Labs Backpack
- Price: $29.99

### Test Steps

1. Navigate to the Products page.
2. Locate the Sauce Labs Backpack.
3. Note the product name and price.
4. Click **Add to cart**.
5. Open the shopping cart.
6. Compare the product name and price in the cart with the information displayed on the Products page.

### Expected Result

The cart should display the same product name and price as shown on the Products page.

### Actual Result

The product name and price displayed in the cart were unchanged from the Products page. The Sauce Labs Backpack was displayed at the correct price of $29.99.

### Status

Pass



## TC-CHECKOUT-001 — Proceed to Checkout

**Test ID:** TC-CHECKOUT-001

**Test Case:** Verify that a user can proceed from the cart to checkout.

**Module:** Checkout

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- At least one product has been added to the cart.
- User is viewing the shopping cart.

**Test Data:**

- Product: Sauce Labs Backpack
- Price: $29.99

### Test Steps

1. Open the shopping cart.
2. Verify that the selected product is displayed.
3. Click the **Checkout** button.
4. Observe the checkout page.

### Expected Result

The user should be directed to the checkout information page, where the required checkout fields are displayed.

### Actual Result

Clicking **Checkout** opened the checkout information page and displayed the **First Name, Last Name, and Postal Code** fields.

### Status

Pass




## TC-CHECKOUT-002 — First Name Is Required

**Test ID:** TC-CHECKOUT-002

**Test Case:** Verify that checkout cannot proceed when the First Name field is empty.

**Module:** Checkout

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- At least one product has been added to the cart.
- User is on the checkout information page.

**Test Data:**

- First Name: Empty
- Last Name: Valid
- Postal Code: Valid

### Test Steps

1. Open the shopping cart.
2. Click the **Checkout** button.
3. Leave the **First Name** field empty.
4. Enter a valid last name.
5. Enter a valid postal code.
6. Click **Continue**.

### Expected Result

The system should prevent the user from proceeding and display the validation message **"First Name is required."**

### Actual Result

The system prevented the user from proceeding and displayed the validation message **"First Name is required."**

### Status

Pass



## TC-CHECKOUT-003 — Last Name Is Required

**Test ID:** TC-CHECKOUT-003

**Test Case:** Verify that checkout cannot proceed when the Last Name field is empty.

**Module:** Checkout

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- At least one product has been added to the cart.
- User is on the checkout information page.

**Test Data:**

- First Name: Valid
- Last Name: Empty
- Postal Code: Valid

### Test Steps

1. Open the shopping cart.
2. Click the **Checkout** button.
3. Enter a valid first name.
4. Leave the **Last Name** field empty.
5. Enter a valid postal code.
6. Click **Continue**.

### Expected Result

The system should prevent the user from proceeding and display the validation message **"Last Name is required."**

### Actual Result

The system prevented the user from proceeding and displayed the validation message **"Last Name is required."**

### Status

Pass


## TC-CHECKOUT-004 — Postal Code Is Required

**Test ID:** TC-CHECKOUT-004

**Test Case:** Verify that checkout cannot proceed when the Postal Code field is empty.

**Module:** Checkout

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- At least one product has been added to the cart.
- User is on the checkout information page.

**Test Data:**

- First Name: Valid
- Last Name: Valid
- Postal Code: Empty

### Test Steps

1. Open the shopping cart.
2. Click the **Checkout** button.
3. Enter a valid first name.
4. Enter a valid last name.
5. Leave the **Postal Code** field empty.
6. Click **Continue**.

### Expected Result

The system should prevent the user from proceeding and display the validation message **"Postal Code is required."**

### Actual Result

The system prevented the user from proceeding and displayed the validation message **"Postal Code is required."**

### Status

Pass


## TC-CHECKOUT-005 — Proceed With Valid Checkout Information

**Test ID:** TC-CHECKOUT-005

**Test Case:** Verify that a user can proceed to the checkout overview using valid checkout information.

**Module:** Checkout

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- At least one product has been added to the cart.
- User is on the checkout information page.

**Test Data:**

- First Name: Valid
- Last Name: Valid
- Postal Code: Valid

### Test Steps

1. Enter a valid first name.
2. Enter a valid last name.
3. Enter a valid postal code.
4. Click **Continue**.
5. Observe the checkout overview page.

### Expected Result

The user should be successfully redirected to the checkout overview page, where the selected product and relevant order information are displayed.

### Actual Result

The user was successfully redirected to the checkout overview page. The product was displayed with its quantity, description, and price. Payment information, shipping information, and the total price were also displayed.

### Status

Pass


## TC-CHECKOUT-006 — Checkout Summary Displays Selected Product

**Test ID:** TC-CHECKOUT-006

**Test Case:** Verify that the checkout overview displays the correct product information.

**Module:** Checkout

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- A product has been added to the cart.
- User has provided valid checkout information.
- User is on the checkout overview page.

**Test Data:**

- Product: Sauce Labs Backpack
- Quantity: 1
- Price: $29.99

### Test Steps

1. Add the Sauce Labs Backpack to the cart.
2. Proceed to checkout.
3. Enter valid First Name, Last Name, and Postal Code.
4. Click **Continue**.
5. Observe the checkout overview.
6. Compare the product name, quantity, description, and price with the information previously displayed for the product.

### Expected Result

The checkout overview should display the correct product name, quantity, description, and price.

### Actual Result

The checkout overview displayed the same product name, quantity, description, and price as previously displayed.

### Status

Pass


## TC-CHECKOUT-007 — Checkout Summary Displays Pricing Information

**Test ID:** TC-CHECKOUT-007

**Test Case:** Verify that the checkout overview displays the correct pricing information.

**Module:** Checkout

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- A product has been added to the cart.
- User has provided valid checkout information.
- User is on the checkout overview page.

**Test Data:**

- Product: Sauce Labs Backpack
- Price: $29.99

### Test Steps

1. Add the Sauce Labs Backpack to the cart.
2. Proceed to checkout.
3. Enter valid First Name, Last Name, and Postal Code.
4. Click **Continue**.
5. Observe the pricing information on the checkout overview page.
6. Verify that the item price, price total, and final total are displayed.

### Expected Result

The checkout overview should display the item price, price total, and final total, including the applicable tax.

### Actual Result

The checkout overview displayed an item total of $29.99, tax of $2.40, and a final total of $32.39. The final total was calculated correctly as the item total plus tax ($29.99 + $2.40 = $32.39).


### Status

Pass


## TC-CHECKOUT-008 — Complete an Order

**Test ID:** TC-CHECKOUT-008

**Test Case:** Verify that a user can successfully complete an order.

**Module:** Checkout

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- At least one product has been added to the cart.
- User has provided valid checkout information.
- User is on the checkout overview page.

**Test Data:**

- Valid checkout information
- Selected product(s)

### Test Steps

1. Proceed through checkout using valid information.
2. Review the checkout overview.
3. Click the **Finish** button.
4. Observe the resulting page.

### Expected Result

The order should be successfully completed and the user should be redirected to the order confirmation page displaying a confirmation message.

### Actual Result

The order was successfully completed. The user was redirected to the **Checkout: Complete!** page, which displayed the confirmation message **"Thank you for your order!"**

### Status

Pass


## TC-PDF-001 — Generate Order PDF

**Test ID:** TC-PDF-001

**Test Case:** Verify that the system generates a PDF containing the order details.

**Module:** Order PDF

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- An order has been completed successfully.
- User is on the Checkout: Complete! page.

**Test Data:**

- Completed order with selected product(s).

### Test Steps

1. Complete an order successfully.
2. On the Checkout: Complete! page, click **Generate PDF order**.
3. Observe the system response.
4. Verify that the generated PDF opens.
5. Verify that the PDF is downloaded.

### Expected Result

The system should generate the order as a PDF. The PDF should open successfully and be downloaded without errors.

### Actual Result

The order PDF was generated successfully. The PDF opened and was downloaded successfully.

### Status

Pass





## TC-PDF-002 — Verify PDF Order Information

**Test ID:** TC-PDF-002

**Test Case:** Verify that the generated PDF contains accurate order information.

**Module:** Order PDF

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- An order has been completed successfully.
- The order PDF has been generated and downloaded.

**Test Data:**

- Product: Sauce Labs Backpack
- Product Price: $29.99
- Item Total: $29.99
- Tax: $2.40
- Final Total: $32.39

### Test Steps

1. Complete an order for the Sauce Labs Backpack.
2. Generate the order PDF.
3. Open the downloaded PDF.
4. Verify the product name.
5. Verify the product price.
6. Verify the item total.
7. Verify the tax.
8. Verify the final total.
9. Compare the information in the PDF with the checkout information.

### Expected Result

The downloaded PDF should contain accurate order information matching the completed order, including the product name, price, item total, tax, and final total.

### Actual Result

The PDF displayed the correct order information:

- Product: Sauce Labs Backpack
- Price: $29.99
- Item Total: $29.99
- Tax: $2.40
- Total: $32.39

The information matched the completed order.

### Status

Pass




## TC-RESET-001 — Reset App State Restores Default State

**Test ID:** TC-RESET-001

**Test Case:** Verify that the Reset App State function restores the application to its expected default state.

**Module:** Application State Management

**Priority:** High

**Preconditions:**

- User is logged in successfully.
- User is on the Products page.
- At least one product is available.

**Test Data:**

- Product: Sauce Labs Backpack

### Test Steps

1. Log in to the SauceDemo application.
2. Add the Sauce Labs Backpack to the cart.
3. Verify that the product displays **Remove**.
4. Open the side menu.
5. Click **Reset App State**.
6. Open the shopping cart.
7. Verify that the cart is empty.
8. Return to the Products page.
9. Observe the button for the Sauce Labs Backpack.

### Expected Result

The Reset App State function should clear the cart and restore the previously added product to its default state, displaying **Add to cart**.

### Actual Result

The cart was successfully cleared after clicking **Reset App State**. However, the Sauce Labs Backpack continued to display **Remove** instead of **Add to cart**. The button only changed to **Add to cart** after manually refreshing the page.

### Status

Fail

### Defect Summary

**Reset App State does not immediately update the product button to its default state.**



















