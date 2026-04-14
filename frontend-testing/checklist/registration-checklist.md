# ✅ Registration Checklist

This checklist covers functional, validation, UI/UX, and security testing of the registration feature.

---

## 🔹 1. Functional Testing

| ID | Test Description | Status | Notes |
|----|-----------------|--------|------|
| 1.1 | "I'm here to buy" and "I'm here to sell" buttons work correctly | Passed | Switching mode |
| 1.2 | Email field is required | Passed | Validation shown when empty |
| 1.3 | Password field is required | Passed | Validation shown when empty |
| 1.4 | "Create Account" button disabled when fields are empty | Passed | |
| 1.5 | "Create Account" button activates with valid data | ❌ Failed | |
| 1.6 | Error appears for invalid email | Passed | e.g. "test@", "user.com" |
| 1.7 | Password validation works | Passed | |
| 1.8 | Password visibility toggle works | Passed | |
| 1.9 | Registration successful with valid data | Passed | |
| 1.10 | Login possible after registration | Passed | |

---

## 🔹 2. Email Validation

| ID | Test Description | Status |
|----|-----------------|--------|
| 2.1 | Email without "@" shows error | Passed |
| 2.2 | Email without domain shows error | Passed |
| 2.3 | Invalid format email shows error | Passed |
| 2.4 | Email with spaces shows error | Passed |
| 2.5 | Invalid special characters show error | Passed |
| 2.6 | Valid email format accepted | Passed |

---

## 🔹 3. Password Validation

| ID | Test Description | Status |
|----|-----------------|--------|
| 3.1 | No uppercase letter | Passed |
| 3.2 | No lowercase letter | Passed |
| 3.3 | No number | Passed |
| 3.4 | Less than 8 characters | Passed |
| 3.9 | No special characters | Passed |
| 3.10 | Valid special characters accepted | Passed |
| 3.11 | Spaces not allowed | Passed |
| 3.12 | Show/hide password works | Passed |

---

## 🔹 4. UI/UX Testing

| ID | Test Description | Status | Notes |
|----|-----------------|--------|------|
| 4.1 | UI elements display correctly | Passed | |
| 4.2 | Validation errors highlighted and disappear after fix | Passed | |
| 4.3 | Keyboard navigation (Tab/Enter) | ❌ Failed | |
| 4.4 | "Log in" button works | Passed | |
| 4.5 | OAuth buttons open correctly | ❌ Failed | |

---

## 🔹 5. Security Testing

| ID | Test Description |
|----|-----------------|
| 5.1 | SQL injection attempts |
| 5.2 | XSS attacks |
| 5.3 | Existing email validation |
| 5.4 | Password storage security |

---

## 🔹 6. Responsiveness

| ID | Test Description | Status |
|----|-----------------|--------|
| 6.1 | Works across browsers | Passed |
| 6.2 | Works on mobile devices | Passed |
| 6.3 | Input fields visible on mobile | Passed |
| 6.4 | Error text readable | Passed |

---

## ⚠️ Notes

- Some issues were identified during testing (see failed cases)
- Testing was based on UI behavior and available requirements

📄 Original version: [PDF](original/Abra_registration.pdf)
