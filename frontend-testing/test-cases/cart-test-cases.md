#  Cart Test Cases

This document contains selected test cases for **shopping cart functionality** in the Abra Market web application.

The scope covers:
- adding products to cart
- cart icon update
- removing products
- total amount calculation
- quantity validation
- checkout flow
- navigation from cart
- mobile behavior

---

## 🔹 Core Test Cases

| ID | Title | Priority | Status |
|----|-------|----------|--------|
| TC1 | Adding a product to the cart | Smoke | ❌ Failed |
| TC2 | Checking the cart icon counter | Critical | Passed |
| TC3 | Removing a product from the cart | Critical | Passed |
| TC4 | Checking the total amount | Critical | ❌ Failed |
| TC5 | Updating product quantity using "+" / "-" buttons | Critical | Passed |
| TC6 | Reaching the minimum quantity | Critical | Passed |
| TC7 | Reaching the maximum quantity | Critical | Passed |
| TC8 | Validation of product quantity = 0 | Critical | Passed |
| TC9 | Validation of negative quantity | Critical | Passed |
| TC10 | Validation of too large quantity | Critical | Passed |
| TC11 | Validation of letters in quantity field | Critical | Passed |
| TC12 | Validation of symbols in quantity field | Critical | Passed |
| TC13 | Continue Shopping button | Critical | Passed |
| TC14 | Checkout button | Smoke | Passed |
| TC15 | Navigation from cart to product page | Smoke | Passed |
| TC16 | Navigation from cart to seller page | Critical | ❌ Failed |
| TC17 | Cart preservation after logout/login | Critical | Passed |
| TC18 | Cart is cleared after placing an order | Critical | ❌ Failed |
| TC19 | Only authorized users can add products to cart | Critical | Not executed / no final status |
| TC20 | Mobile interface adaptation | Critical | Not executed / no final status |
| TC21 | Adding products to cart on mobile | Smoke | Not executed / no final status |
| TC22 | Removing products from cart on mobile | Critical | Not executed / no final status |
| TC23 | Placing an order on mobile | Smoke | Not executed / no final status |

---

## 🔹 Key Failed Scenarios

### TC1 — Adding a Product to the Cart
**Expected:** product is added to cart with correct details.  
**Actual:** test failed during execution.

### TC4 — Checking the Total Amount
**Expected:** total amount = sum of all product prices × quantity.  
**Actual:** total amount calculation was incorrect.

### TC16 — Navigating from Cart to Seller Page
**Expected:** clicking seller name opens seller page.  
**Actual:** navigation did not work as expected.

### TC18 — Clearing the Cart After Placing an Order
**Expected:** after successful order placement, the cart should be empty.  
**Actual:** cart was not cleared after order completion.

---

## 🔹 Validation Coverage

The cart test cases include validation of:
- minimum quantity
- maximum quantity
- zero value
- negative values
- letters
- symbols

This helped verify input restrictions and quantity handling logic.

---

## 🔹 Notes

- Some failed scenarios were later used as a basis for bug reconstruction.
- Part of the quantity-related testing required manual input into the field before clicking action buttons.

---

📄 Original version: [PDF](original/cart-test-cases.pdf)
