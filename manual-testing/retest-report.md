# SauceDemo — Retest & Regression Test Report

## 1. Purpose

This report documents the retesting of previously failed test cases and
the regression testing performed on related application functionality.

The purpose of the retest was to determine whether the previously
identified defects were still reproducible in the current version of the
application.

---

## 2. Retest Scope

The following previously failed scenarios were selected for retesting:

| Test ID | Defect | Area |
|---|---|---|
| TC-LOGIN-008 | Incorrect login redirection | Login |
| TC-PRODUCT-004 | Incorrect product information | Product Details |
| TC-PRODUCT-006 | Product sorting failure | Product Browsing |
| TC-RESET-001 | Reset App State UI inconsistency | Application State |

---

## 3. Retest Environment

| Item | Details |
|---|---|
| Application | SauceDemo |
| Operating System | macOS |
| Browser | Google Chrome |
| Testing Type | Manual Retesting |
| Test Environment | Web |

---

# 4. Retest Results

## TC-LOGIN-008 — Login Redirect

### Original Result

**Fail**

The `performance_glitch_user` account was successfully authenticated,
but the application redirected the user to a Product Details page
instead of the Products page.

### Retest Steps

1. Open the SauceDemo application.
2. Log in using `performance_glitch_user`.
3. Enter the valid password.
4. Click Login.
5. Observe the page displayed after authentication.

### Retest Result

**Fail**

### Observation

The user was successfully authenticated but was redirected to a Product
Details page instead of the Products page.

### Defect Status

**Still Open**

### Related Defect

BUG-004

---

## TC-PRODUCT-004 — Product Details Information

### Original Result

**Fail**

The Product Details page displayed incorrect product information when
using the `problem_user` account.

### Retest Steps

1. Log in using `problem_user`.
2. Navigate to the Products page.
3. Locate the Sauce Labs Backpack.
4. Note its product information.
5. Open the product details.
6. Compare the information with the Products page.

### Retest Result

**Fail**

### Observation

The Product Details page continued to display incorrect product
information compared with the selected product.

### Defect Status

**Still Open**

### Related Defect

BUG-001

---

## TC-PRODUCT-006 — Product Sorting

### Original Result

**Fail**

Product sorting did not work correctly for the affected test accounts.

### Retest Steps

1. Log in using `problem_user`.
2. Navigate to the Products page.
3. Select a sorting option.
4. Observe the product order.
5. Repeat the test using `error_user`.

### Retest Result

**Fail**

### Observation

The sorting functionality continued to behave incorrectly.

With `problem_user`, selecting a sorting option did not change the
product order.

With `error_user`, the application displayed:

"Sorting is broken! This error has been reported to Backtrace."

### Defect Status

**Still Open**

### Related Defect

BUG-002

---

## TC-RESET-001 — Reset App State

### Original Result

**Fail**

Reset App State cleared the cart but did not immediately update the
product button from **Remove** to **Add to cart**.

### Retest Steps

1. Log in to the application.
2. Add the Sauce Labs Backpack to the cart.
3. Verify that the button displays **Remove**.
4. Open the side menu.
5. Select **Reset App State**.
6. Open the cart and verify that it is empty.
7. Return to the Products page.
8. Observe the product button.

### Retest Result

**Fail**

### Observation

The cart was cleared, but the product button continued to display
**Remove** until the page was manually refreshed.

### Defect Status

**Still Open**

### Related Defect

BUG-003

---

# 5. Retest Summary

| Test ID | Original | Retest | Defect Status |
|---|---|---|---|
| TC-LOGIN-008 | Fail | Fail | Open |
| TC-PRODUCT-004 | Fail | Fail | Open |
| TC-PRODUCT-006 | Fail | Fail | Open |
| TC-RESET-001 | Fail | Fail | Open |

### Retest Outcome

**4 of 4 previously failed scenarios remain reproducible.**

No previously identified defect was confirmed as resolved during this
retest cycle.

---

# 6. Regression Testing

Regression testing was performed on related core functionality to ensure
that the observed issues did not prevent other major application
workflows from functioning.

The following areas were checked:

- Login
- Product browsing
- Shopping cart
- Checkout
- Order completion
- Order PDF generation

The core shopping and checkout workflows continued to function as
expected during the regression check.

---

# 7. Regression Result

**Regression Status: Pass with Known Defects**

The application's primary shopping and checkout workflows remain
functional.

However, the previously reported defects remain unresolved and should
be addressed before the affected functionality is considered ready for
release.

---

# 8. Final Recommendation

The application should undergo another retest cycle after the identified
defects are addressed.

The following defects remain open:

- BUG-001 — Incorrect product information
- BUG-002 — Product sorting failure
- BUG-003 — Reset App State UI inconsistency
- BUG-004 — Incorrect login redirection

A new regression cycle should be performed after fixes are implemented.
