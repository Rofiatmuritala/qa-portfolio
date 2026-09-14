# SauceDemo — Test Execution Report

## 1. Test Execution Overview

This test execution was performed to evaluate the core functionality of
the SauceDemo e-commerce web application.

The testing covered authentication, product browsing, product details,
product sorting, shopping cart functionality, checkout, order completion,
order PDF generation, and application state management.

Testing was performed using functional, positive, negative, and
exploratory testing techniques.

---

## 2. Test Environment

| Environment | Details |
|---|---|
| Application | SauceDemo |
| Operating System | macOS |
| Browser | Google Chrome |
| Testing Type | Manual Testing |
| Test Execution | Functional Testing |
| Primary Device | Laptop |

---

## 3. Test Execution Summary

| Metric | Result |
|---|---:|
| Total Test Cases | 35 |
| Passed | 31 |
| Failed | 4 |
| Pass Rate | 88.57% |
| Fail Rate | 11.43% |

### Overall Result

**Test execution completed with 31 passed and 4 failed test cases.**

The application successfully passed the majority of the planned functional
tests. However, several defects were identified in product details,
product sorting, application state reset, and login redirection.

---

## 4. Test Results by Module

| Module | Total | Passed | Failed |
|---|---:|---:|---:|
| Login & Authentication | 10 | 8 | 2 |
| Product Browsing & Product Details | 6 | 4 | 2 |
| Shopping Cart | 8 | 8 | 0 |
| Checkout | 8 | 8 | 0 |
| Order PDF | 2 | 2 | 0 |
| Application State Management | 1 | 0 | 1 |
| **Total** | **35** | **31** | **4** |

---

## 5. Failed Test Cases

### TC-LOGIN-008 — Successful Login Redirects to Products Page

**Result:** Fail

**Observed Issue:**

The `performance_glitch_user` account was successfully authenticated,
but instead of being redirected to the Products page, the application
redirected the user to a Product Details page.

**Defect:** Login redirection does not behave as expected for the
performance glitch user.

---

### TC-PRODUCT-004 — Product Details Contain Correct Information

**Result:** Fail

**Observed Issue:**

When testing with the `problem_user` account, selecting the Sauce Labs
Backpack from the Products page opened a Product Details page displaying
Sauce Labs Fleece Jacket at $49.99 with a different image.

**Defect:** Product details do not correspond to the selected product.

**Related Defect:** BUG-001

---

### TC-PRODUCT-006 — Product Sorting

**Result:** Fail

**Observed Issue:**

When using the `problem_user` account, selecting a sorting option did not
change the product order.

When using the `error_user` account, selecting a sorting option displayed
the error message:

"Sorting is broken! This error has been reported to Backtrace."

**Defect:** Product sorting functionality does not work correctly for the
affected test accounts.

**Related Defect:** BUG-002

---

### TC-RESET-001 — Reset App State Restores Default State

**Result:** Fail

**Observed Issue:**

After selecting Reset App State, the cart was successfully cleared.
However, the Sauce Labs Backpack button continued to display **Remove**
instead of **Add to cart**.

The button changed to **Add to cart** only after manually refreshing the
page.

**Defect:** Reset App State does not immediately update the product button
state.

**Related Defect:** BUG-003

---

## 6. Defect Summary

| Defect ID | Description | Severity | Priority | Status |
|---|---|---|---|---|
| BUG-001 | Product Details displays incorrect product information | Medium | High | Open |
| BUG-002 | Product sorting functionality does not work | Medium | Medium | Open |
| BUG-003 | Reset App State does not immediately update product button state | Medium | Medium | Open |
| BUG-004 | Login redirects to incorrect page for performance glitch user | Medium | High | Open |

---

## 7. Passed Functional Areas

The following areas completed testing without identified failures:

- Valid login
- Invalid login credentials
- Empty login fields
- Locked-out user handling
- Logout
- Product listing
- Opening product details under normal conditions
- Returning from Product Details to Products
- Adding products to cart
- Adding multiple products
- Cart count updates
- Removing products
- Continuing shopping
- Checkout validation
- Checkout overview
- Pricing calculations
- Order completion
- Order PDF generation
- Order PDF information accuracy

---

## 8. Testing Observations

The core shopping and checkout workflows performed successfully during
the test execution.

The main issues identified were concentrated around specific test
accounts and application state synchronization.

The identified failures should be investigated, corrected, and retested
before the affected functionality is considered ready for release.

---

## 9. Release Recommendation

### Recommendation: Conditional Release

The application demonstrated generally stable core shopping and checkout
functionality, with 88.57% of executed test cases passing.

However, the identified defects should be reviewed and prioritized before
release, particularly the defects affecting product information,
application state, sorting, and login redirection.

A regression test should be performed after the defects are fixed.
