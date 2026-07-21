# Day 6 - Test Case Design & Bug Reporting

## Topics Covered

- Learned the structure of a professional test case.
- Wrote 5 test cases for the Cart Page.
- Identified UI/UX improvement suggestions.
- Practiced writing professional bug reports.
- Answered common QA interview questions.

## Deliverables

- ✅ 5 Cart Page Test Cases
- ✅ 2 UI/UX Improvement Suggestions
- ✅ 2 Bug Reports
- ✅ 4 Interview Questions

## Website Tested

https://www.saucedemo.com

## Testing Environment

- Browser: Google Chrome
- OS: Windows 11

## Key Learnings

- Difference between Severity and Priority
- Difference between Verification and Validation
- Writing clear bug reports
- Creating professional test cases















## Cart test cases
# Cart Page Test Cases

---

## TC001 - Verify Remove Button Functionality

**Precondition**

- User is logged into the application.
- User has at least one product in the cart.
- User is on the Cart page.

**Steps**

1. Login with valid credentials.
2. Add a product to the cart.
3. Open the Cart page.
4. Click the **Remove** button.

**Test Data**

N/A

**Expected Result**

Selected item should be removed from the cart.

**Actual Result**

Selected item was removed successfully.

**Status**

Pass

---

## TC002 - Verify Product Details

**Precondition**

- User is logged into the application.
- At least one product is added to the cart.

**Steps**

1. Login with valid credentials.
2. Add a product to the cart.
3. Open the Cart page.
4. Click the product name.

**Test Data**

N/A

**Expected Result**

Product details page should display the correct product name, description, image, and price.

**Actual Result**

Correct product details were displayed.

**Status**

Pass

---

## TC003 - Verify Continue Shopping Button

**Precondition**

- User is logged into the application.
- User is on the Cart page.

**Steps**

1. Login with valid credentials.
2. Open the Cart page.
3. Click **Continue Shopping**.

**Test Data**

N/A

**Expected Result**

User should be redirected to the Inventory page.

**Actual Result**

Inventory page opened successfully.

**Status**

Pass

---

## TC004 - Verify Checkout Button

**Precondition**

- User is logged into the application.
- At least one product is present in the cart.

**Steps**

1. Login with valid credentials.
2. Add a product to the cart.
3. Open the Cart page.
4. Click the **Checkout** button.

**Test Data**

N/A

**Expected Result**

Checkout Information page should open.

**Actual Result**

Checkout Information page opened successfully.

**Status**

Pass

---

## TC005 - Verify Product Quantity Display

**Precondition**

- User is logged into the application.
- At least one product is added to the cart.

**Steps**

1. Login with valid credentials.
2. Add a product to the cart.
3. Open the Cart page.

**Test Data**

N/A

**Expected Result**

The quantity displayed for the added product should be correct.

**Actual Result**

Quantity displayed correctly as 1.

**Status**

Pass



## Bug Report

# Bug Reports

---

## Bug Report 1

**Bug ID**

BUG001

**Title**

Checkout button is unresponsive after clicking.

**Severity**

High

**Priority**

High

**Environment**

- Browser: Google Chrome
- OS: Windows 11

**Steps to Reproduce**

1. Open SauceDemo.
2. Login using valid credentials.
3. Add at least one product to the cart.
4. Open the Cart page.
5. Click the **Checkout** button.

**Expected Result**

User should be redirected to the Checkout Information page.

**Actual Result**

Clicking the Checkout button produces no response, and the user remains on the Cart page.

**Status**

Open

---

## Bug Report 2

**Bug ID**

BUG002

**Title**

Cart badge count is not updated after removing all items.

**Severity**

High

**Priority**

High

**Environment**

- Browser: Google Chrome
- OS: Windows 11

**Steps to Reproduce**

1. Open SauceDemo.
2. Login using valid credentials.
3. Add three products to the cart.
4. Open the Cart page.
5. Remove all products.
6. Observe the cart badge.

**Expected Result**

All products should be removed successfully, and the cart badge should disappear or display "0".

**Actual Result**

All products are removed successfully; however, the cart badge continues to display "3".

**Status**

## Interview Questions

# QA Interview Questions - Day 6

## Q1. Difference between Verification and Validation

### Verification

Verification checks whether the software is being developed according to the requirements and design.

**Question Answered**

> Are we building the product right?

### Validation

Validation checks whether the final product satisfies customer requirements.

**Question Answered**

> Are we building the right product?

### Example

A customer orders a red dirt bike.

- **Verification:** Check whether the engine, brakes, wheels, and other components are assembled correctly according to the design.
- **Validation:** Verify that the final bike is a red dirt bike as requested by the customer.

---

## Q2. What makes a good bug report?

A good bug report should be:

- Clear and easy to understand
- Easy to reproduce
- Include environment details
- Mention severity and priority
- Include expected and actual results
- Contain screenshots or videos if required

---

## Q3. Who decides bug priority?

Bug priority is generally decided by the Product Manager, Project Manager, Client, or Product Owner based on business impact.

The QA team may recommend a priority, but the final decision is usually made by the business or product team.

---

## Q4. Can a low-severity bug have high priority?

Yes.

### Example

A spelling mistake on the homepage.

- Severity: Low
- Priority: High

Although it does not affect functionality, it is visible to every user and should be fixed quickly.