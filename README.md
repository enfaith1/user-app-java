# Simple User Management Application (Java Swing)

This Java Swing application provides basic user login and management functionalities. It allows users to log in, add, update, and manage user accounts stored in a JSON file.

## Overview

The application consists of several Java classes:

* **`login.java`:** Handles user login, reading user credentials from `user.json` and validating them.
* **`welcome.java`:** Displays a welcome screen after successful login and provides buttons for user management actions.
* **`add.java`:** Allows adding new user accounts to the `user.json` file.
* **`update.java`:** Enables updating existing user account information in the `user.json` file.
* **`user.json`:** Stores user credentials in JSON format.

## Functionality

1.  **Login:**
    * Users enter their username and password.
    * The application reads user data from `user.json`.
    * Credentials are validated, and if correct, the user is directed to the welcome screen.

2.  **User Management (Welcome Screen):**
    * Provides options to add, update, or log out.

3.  **Add User:**
    * Users can enter a new username and password.
    * The application checks for duplicate usernames.
    * New user data is added to `user.json`.

4.  **Update User:**
    * Users can update existing user credentials by providing the current username, new username, and new password.
    * The application searches for the user and updates the information.

5.  **Data Storage:**
    * User data is stored in a JSON file (`user.json`).

## How to Run

1.  **Prerequisites:**
    * Java Development Kit (JDK) installed.
    * `json-simple` library added to the project's classpath.
      
2.  **Installation:**
    * Clone or download the project.
    * Open the project in your Java IDE.
    * Ensure the `json-simple` library is added to the project's build path.
    * Verify the `user.json` file is correctly located in `src/Login/`.

3.  **Running the Application:**
    * Run the `login.java` file to start the application.

## Security Considerations

* **Password Storage:** Currently, passwords are stored in plain text in the `user.json` file. This is a significant security risk.
* **Recommendations:**
    * Implement password hashing (e.g., bcrypt, Argon2) to store passwords securely.
    * Consider using a database for more robust user management.

## Potential Improvements

* **Password Security:** Implement password hashing.
* **Error Handling:** Add more comprehensive error handling and user feedback.
* **Input Validation:** Add input validation to prevent invalid characters and enforce password complexity.
* **UI/UX:** Improve the user interface and user experience.
* **Code Organization:** Refactor the code for better organization and maintainability.
* **File Path Configuration:** Make the `user.json` file path configurable.
* **Robust File handling:** add try catch blocks around file read and write operations.
* **Session Management:** Implement session management for better security.
