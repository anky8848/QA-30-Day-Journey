# Day 4 Notes

## Can Software Be 100% Bug-Free?

**No.** Software can never be guaranteed to be 100% bug-free because it is impossible to test every possible scenario, input, device, browser, and user behavior.

Testing helps identify defects and reduce risk, but it cannot prove that no defects remain.

**Key Points**
- Exhaustive testing is impossible.
- QA reduces risk, not eliminates it.
- Some bugs may still appear after release.
- The goal is to deliver reliable and high-quality software.

---

# The 7 Testing Principles (ISTQB)

## 1. Testing Shows the Presence of Defects
Testing can prove that defects exist, but it cannot prove that software is completely bug-free.

**Example:** Even if 1000 test cases pass, an undiscovered bug may still exist.

---

## 2. Exhaustive Testing is Impossible
Testing every possible input, combination, and scenario is impossible.

Instead, testers prioritize important and high-risk areas.

**Example:** A login page has millions of possible username and password combinations.

---

## 3. Early Testing Saves Time and Cost
Testing should begin as early as possible during the Software Development Life Cycle (SDLC).

Finding defects in requirements or design is much cheaper than fixing them after development.

---

## 4. Defect Clustering
Most defects are usually found in a small number of modules.

This follows the Pareto Principle (80/20 Rule):
- Around 80% of defects are found in 20% of the application.

---

## 5. Pesticide Paradox
Running the same test cases repeatedly eventually stops finding new defects.

Test cases should be reviewed, updated, and expanded regularly.

---

## 6. Testing is Context-Dependent
Different applications require different testing approaches.

**Example:**
- Banking software requires high security and accuracy.
- A game focuses more on performance and user experience.

---

## 7. Absence-of-Errors Fallacy
Even software with no known defects can fail if it does not meet user or business requirements.

Bug-free software is not useful if it does not solve the intended problem.

---

# Memory Trick

**P E E D P C A**

- **P** – Presence of Defects
- **E** – Exhaustive Testing
- **E** – Early Testing
- **D** – Defect Clustering
- **P** – Pesticide Paradox
- **C** – Context-Dependent Testing
- **A** – Absence-of-Errors Fallacy

---

# QA Throughout the SDLC

A QA Engineer contributes throughout the Software Development Life Cycle, not just after development is completed.

### Responsibilities

- Review requirements
- Identify ambiguities
- Plan testing early
- Design test cases
- Execute testing
- Validate bug fixes
- Support product releases

**Goal:** Prevent defects early instead of only finding them later.

---

# QA vs Bug Bounty

| QA Engineer | Bug Bounty Hunter |
|-------------|-------------------|
| Tests software quality | Finds security vulnerabilities |
| Focuses on functionality, usability, performance, compatibility | Focuses on application security |
| Works before release | Usually tests authorized live applications |
| Reports defects to the development team | Reports security vulnerabilities through bug bounty programs |

A QA Engineer can transition into Security Testing or Bug Bounty by learning:
- OWASP Top 10
- API Security
- Burp Suite
- Authentication & Authorization
- Common Web Vulnerabilities

---

# Practical Task Understanding

For practice websites like SauceDemo and OrangeHRM:

The objective is **not** to find bugs.

Instead:

- Explore the application.
- Understand its features.
- Identify major modules.
- Decide what should be tested first as a QA Engineer.

This develops analytical thinking before writing test cases.

---

# Creating Your Own Bugs

When asked to "Create your own 5 bugs," it means creating **realistic hypothetical bug scenarios**, not finding actual defects.

Each bug should include:

- Bug Description
- Severity
- Priority

### Example

**Bug:** Login button does not work with valid credentials.

**Severity:** Critical

**Priority:** High

---

# Key Takeaways

- Software cannot be guaranteed to be bug-free.
- Testing reduces risk but cannot eliminate all defects.
- Learn and remember the 7 ISTQB Testing Principles.
- QA participates throughout the SDLC.
- Practical tasks are meant to build a QA mindset.
- Bug scenarios can be hypothetical for learning purposes.





## TAsk 1
| S.N. | Test Scenario                                                 | Result | Remarks                                                                                                                                          |
| ---- | ------------------------------------------------------------- | ------ | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1    | Verify the Inventory page loads successfully after login.     | ✅ Pass | Inventory page loaded successfully.                                                                                                              |
| 2    | Verify all product names are displayed.                       | ✅ Pass | All product names are visible.                                                                                                                   |
| 3    | Verify all product prices are displayed correctly.            | ✅ Pass | Prices are displayed for all products.                                                                                                           |
| 4    | Verify the **Add to Cart** button works for all products.     | ❌ Fail | Only **3 out of 6** Add to Cart buttons work. The remaining buttons do not respond.                                                              |
| 5    | Verify the **Remove** button works after adding a product.    | ❌ Fail | Remove button appears but does not remove the product.                                                                                           |
| 6    | Verify the shopping cart badge updates after adding products. | ✅ Pass | Cart badge updates correctly when products are added.                                                                                            |
| 7    | Verify product sorting works (A–Z, Z–A, Low–High, High–Low).  | ❌ Fail | Only the default **A–Z** sorting works. Other sorting options do not work.                                                                       |
| 8    | Verify product images are displayed correctly.                | ✅ Pass | All product images are displayed correctly.                                                                                                      |
| 9    | Verify clicking the cart icon opens the Cart page.            | ✅ Pass | Cart page opens successfully.                                                                                                                    |
| 10   | Verify the checkout process works correctly.                  | ❌ Fail | Last Name field does not accept input. Finish button is not working. First Name and Postal Code fields work correctly. Logout works as expected. |


## Task 2 
# Day 4 - Test Cases (SauceDemo)

| Test Case ID | Module | Title | Preconditions | Test Steps | Expected Result | Actual Result | Status |
|--------------|--------|-------|----------------|------------|-----------------|---------------|--------|
| TC001 | Inventory | Verify the Inventory page loads successfully after login. | User is on the Login page with valid credentials. | 1. Enter a valid username.<br>2. Enter a valid password.<br>3. Click the **Login** button. | The Inventory page should load successfully and display all inventory items. |  |  |
| TC002 | Inventory | Verify all product names are displayed. | User is logged in and on the Inventory page. | 1. Login with valid credentials.<br>2. Navigate to the Inventory page.<br>3. Observe the product list. | All product names should be displayed correctly. |  |  |
| TC003 | Product Pricing | Verify all product prices are displayed correctly. | User is logged in and on the Inventory page. | 1. Login with valid credentials.<br>2. Navigate to the Inventory page.<br>3. Check the price displayed for each product. | Every product should display its corresponding price correctly. |  |  |
| TC004 | Add to Cart | Verify the **Add to Cart** button works for all products. | User is logged in and on the Inventory page. | 1. Login with valid credentials.<br>2. Click the **Add to Cart** button for each product. | The selected product should be added to the shopping cart successfully, and the button should change to **Remove**. |  |  |
| TC005 | Remove Product | Verify the **Remove** button works after adding a product. | User is logged in, on the Inventory page, and at least one product has been added to the cart. | 1. Login with valid credentials.<br>2. Click **Add to Cart** for any product.<br>3. Click the **Remove** button. | The selected product should be removed from the shopping cart, and the button should change back to **Add to Cart**. |  |  |



## TAsk 3
# Day 4 - Bug Thinking Exercise

| S.N. | Bug | Severity | Priority | Reason |
|------|-----|----------|----------|--------|
| 1 | Product image not loading. | Medium | Medium | Users can still view product details and purchase the item, but the user experience is affected. |
| 2 | Add to Cart button doesn't work. | High | High | Users cannot add products to the cart, preventing purchases. |
| 3 | Logout button missing. | Critical | High | Users cannot securely log out, creating a security and usability issue. |
| 4 | Cart badge count incorrect. | High | High | Incorrect cart information can confuse users and affect the shopping experience. |
| 5 | Product price shown as $0. | High | High | Incorrect pricing may cause financial loss and incorrect orders if users can purchase at that price. |

