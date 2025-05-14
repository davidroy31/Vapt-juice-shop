# Login as Jim – OWASP Juice Shop

This guide explains how to log in as the user **Jim** in the [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/), a deliberately insecure web app for security training, awareness demos, and testing.

## 🧾 Prerequisites

- OWASP Juice Shop instance running locally or remotely.
- Web browser or API client like Postman/cURL.
- Optional: Access to browser dev tools or intercepting proxy (e.g., Burp Suite).

---

## 🔐 Login Details (User: Jim)

The default user **Jim** is one of the demo users included in Juice Shop's seeded data. His credentials are usually:

- **Email:** `jim@juice-sh.op`
- **Password:** `anuj123`

> If these credentials don’t work, the app may have custom seed data or the database was reset. Try solving the “Login Jim” challenge to rediscover the credentials.

---

## 🚀 Login Steps (Web Interface)

1. Open your browser and go to the Juice Shop homepage (e.g., `http://localhost:3000`).
2. Click the **"Account"** icon in the top right corner.
3. Choose **"Login"** from the dropdown.
4. Enter the following credentials:

   - **Email:** `jim@juice-sh.op`
   - **Password:** `anuj123`

5. Click **"Log in"**.

You should now be logged in as Jim. Check for any relevant challenge solved notifications.

---

## 🧪 Login via API (Optional)

You can also log in via the REST API:

### Request

```http
POST /rest/user/login HTTP/1.1
Host: localhost:3000
Content-Type: application/json

{
  "email": "jim@juice-sh.op",
  "password": "anuj123"
}
