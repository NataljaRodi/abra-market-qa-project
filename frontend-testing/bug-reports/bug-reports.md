# 🐞 Bug Reports

This document contains reconstructed bug reports based on failed test scenarios identified during testing of the Abra Market platform.

The bugs were derived from:
- checklist execution
- test case failures
- API validation issues

---

## 🧾 Summary

| ID | Title | Module | Severity |
|----|------|--------|----------|
| BUG-01 | Create Account button does not activate | Registration | Major |
| BUG-02 | Keyboard navigation does not work correctly | Registration | Medium |
| BUG-03 | Cart total amount is incorrect | Cart | Critical |
| BUG-04 | Seller link in cart does not work | Cart | Major |
| BUG-05 | API accepts negative quantity value | API | Critical |

---

## 🐞 BUG-01 — Create Account button does not activate

**Module:** Registration  
**Severity:** Major  
**Priority:** High  

### 📌 Description
"Create Account" button does not become active even when valid data is entered.

### 🔁 Steps to reproduce
1. Open registration page  
2. Select account type  
3. Enter valid email  
4. Enter valid password  

### ✅ Expected result
Button becomes active.

### ❌ Actual result
Button remains inactive.

### 🔗 Source
Checklist item 1.5

---

## 🐞 BUG-02 — Keyboard navigation does not work correctly

**Module:** Registration  
**Severity:** Medium  
**Priority:** Medium  

### 📌 Description
Keyboard navigation using Tab / Enter is inconsistent.

### 🔁 Steps to reproduce
1. Open registration page  
2. Navigate using keyboard  

### ✅ Expected result
User can navigate all fields using keyboard.

### ❌ Actual result
Navigation does not work correctly.

### 🔗 Source
Checklist item 4.3

---

## 🐞 BUG-03 — Cart total amount is calculated incorrectly

**Module:** Cart  
**Severity:** Critical  
**Priority:** High  

### 📌 Description
Total amount does not match sum of items in cart.

### 🔁 Steps to reproduce
1. Add multiple products  
2. Open cart  

### ✅ Expected result
Total = price × quantity (for all items)

### ❌ Actual result
Incorrect total amount displayed

### ⚠️ Impact
User may see incorrect price before checkout.

### 🔗 Source
Test case TC4

---

## 🐞 BUG-04 — Seller link in cart does not open seller page

**Module:** Cart  
**Severity:** Major  
**Priority:** High  

### 📌 Description
Clicking seller name does not redirect to seller page.

### 🔁 Steps to reproduce
1. Open cart  
2. Click seller name  

### ✅ Expected result
Seller page opens.

### ❌ Actual result
No navigation occurs.

### 🔗 Source
Test case TC16

---

## 🐞 BUG-05 — API accepts negative quantity value

**Module:** API / Cart  
**Severity:** Critical  
**Priority:** High  

### 📌 Description
API accepts invalid negative value instead of returning a validation error.

### 🔁 Steps to reproduce
1. Send request to update product quantity  
2. Set `amount = -1`

### ✅ Expected result
Validation error is returned (for example 422).

### ❌ Actual result
API returns `200 OK` and accepts the invalid value.

### ⚠️ Impact
Invalid data can be saved in cart.

### 🔗 Source
API test case 13

---

## 📌 Notes

- Bug reports were reconstructed based on test results and failed scenarios.
- Original Jira reports are not available due to project access limitations.
