# QA 30-Day Journey — Day 5

## Topic
**Test Scenarios & Test Cases**

---

# Part 2 — Practice (Inventory Page Execution)

**Website:** https://www.saucedemo.com

**Login Credentials**
- Username: `standard_user`
- Password: `secret_sauce`

### Test Scenario Execution

| S.N. | Test Scenario | Status |
|------|---------------|--------|
| 1 | Verify Inventory page loads successfully. | ✅ Pass |
| 2 | Verify all products are displayed. | ✅ Pass |
| 3 | Verify product images are visible. | ✅ Pass |
| 4 | Verify prices are displayed. | ✅ Pass |
| 5 | Verify Add to Cart button works. | ❌ Fail |
| 6 | Verify Remove button appears after adding a product. | ✅ Pass |
| 7 | Verify shopping cart badge updates after adding a product. | ✅ Pass |
| 8 | Verify sorting by Name (A–Z). | ✅ Pass |
| 9 | Verify sorting by Price (Low to High). | ❌ Fail |
| 10 | Verify cart icon opens the Cart page. | ✅ Pass |

### Failed Scenarios

**Scenario 5**
- **Status:** Fail
- **Reason:** Clicking the **Add to Cart** button did not add the selected product to the cart.

**Scenario 9**
- **Status:** Fail
- **Reason:** Products were not sorted correctly after selecting **Price (Low to High)**.

---

# Part 3 — Test Cases

## Test Case 1

| Field | Details |
|-------|---------|
| **Test Case ID** | TC001 |
| **Title** | Verify Add to Cart functionality |
| **Precondition** | User is logged into SauceDemo |
| **Steps** | 1. Open the Inventory page.<br>2. Click the **Add to Cart** button for any product. |
| **Expected Result** | The selected product should be added to the cart, the **Remove** button should appear, and the cart badge count should increase by 1. |
| **Actual Result** | __________ |
| **Status** | Pass / Fail |

---

## Test Case 2

| Field | Details |
|-------|---------|
| **Test Case ID** | TC002 |
| **Title** | Verify Product Sorting |
| **Precondition** | User is logged into SauceDemo |
| **Steps** | 1. Open the Inventory page.<br>2. Click the Sort dropdown.<br>3. Select **Name (A–Z)** and verify the order.<br>4. Repeat for **Name (Z–A)**, **Price (Low to High)**, and **Price (High to Low)**. |
| **Expected Result** | Products should be sorted correctly according to the selected sorting option. |
| **Actual Result** | __________ |
| **Status** | Pass / Fail |

---

## Test Case 3

| Field | Details |
|-------|---------|
| **Test Case ID** | TC003 |
| **Title** | Verify Product Details Page |
| **Precondition** | User is logged into SauceDemo |
| **Steps** | 1. Open the Inventory page.<br>2. Click on any product name or image. |
| **Expected Result** | The product details page should open and display the correct product name, image, description, and price. |
| **Actual Result** | __________ |
| **Status** | Pass / Fail |