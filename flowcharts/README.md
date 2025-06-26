# 🔁 User Registration – Flowchart

This diagram illustrates the user registration process in the Airbnb Clone backend.

## 🖼️ Flowchart

![User Registration Flowchart](./data-flow-diagram.png)

## 🧩 Description

- The process begins when a user submits the registration form.
- The system validates the input and checks for email uniqueness.
- If the data is valid and the email is unused:
  - The password is hashed.
  - A new user is created in the database.
  - A JWT token is generated and returned to the client.
- In case of validation failure or email conflict, appropriate error messages are returned.

This helps visualize the critical validation and decision points during account creation.

