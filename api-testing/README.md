# 🔗 API Testing

This section demonstrates my hands-on experience in API testing using Postman during QA internship on the Abra Market platform.

---

## 📌 Scope

API testing was focused on cart functionality and authentication.

### Covered endpoints

- Add product to cart (PUT)
- Remove product from cart (DELETE)
- Get seller cart (GET)
- Update product quantity (POST)
- Log in / Sign out (POST)

---

## 🧪 Testing Approach

I performed:

- Positive testing
- Negative testing
- Destructive testing

---

## 🧩 Test Structure

The test collection is organized into:

### Positive scenarios
- Valid product addition
- Successful authentication

### Negative scenarios
- Missing parameters
- Invalid data types
- Unauthorized requests

### Destructive scenarios
- SQL injection attempts
- XSS payloads
- Long query strings

---

## 🔹 Example Test

### Add product

PUT /addProduct

amount = 5  
bundle_variation_pod_id = 88  

Expected: product added  

---

## 🛠 Tools

- Postman
- Swagger

---

## 📁 Postman Collection

👉 👉 [View Postman Collection](postman/Abra_cart_tests.postman_collection.json)
