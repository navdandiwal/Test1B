
This project is a JavaFX Login Application created by Navdeep Singh. It includes a login page with username and password fields, and implements login validation, attempt tracking, and account lockout functionality.

Features:
User Interface: A simple JavaFX interface for user login.
User Information Display: Shows the developer's name, student ID, and current date.
Login Validation: Checks if the username and password fields are empty.
Static Login Credentials: Predefined username ("Navdeep") and password ("456") for authentication.
Attempt Counter: Tracks the number of failed login attempts.
Account Lockout: Locks the account after 5 unsuccessful login attempts.
Technologies Used:
JavaFX
Java
How to Run:
Prerequisites: Ensure you have a Java Development Kit (JDK) and an IDE compatible with JavaFX (Replit) installed.
Open Project: Open the project in your IDE.
Run Main Class: Run the Main class.
Project Structure:
Main.java: Contains the main JavaFX application setup, including UI elements and layout.
LoginController.java: Handles the login logic, including validation, credential checking, and managing login attempts.
User.java: A simple class to represent a user with username and password properties.
Code Details:
Main.java (UI Setup)
This class sets up the primary stage for the JavaFX application. It includes:

Labels for "Name: Navdeep Singh", "Student ID: 23094413", and "Date: 2025-06-19".
A "Login Page" title with custom styling.
Text fields for "Username" and "Password".
A "Login" button.
Layouts (VBox) to organize these elements.
Scene and stage setup for displaying the application window.
LoginController.java (Login Logic)
This class manages the login process.

attempts: An integer variable to keep track of failed login attempts.
correctUsername: Set to "Navdeep".
correctPassword: Set to "456".
handleLogin(String username, String password):
Returns "Please Provide Username or Password" if either field is empty.
Returns "Sorry, Your Account is Locked!!!" if attempts is 5 or more.
If credentials match, attempts is reset to 0, and "Success!!!" is returned.
If credentials do not match, attempts is incremented. If attempts reaches 5, "Sorry, Your Account is Locked!!!" is returned; otherwise, "Sorry, Invalid Username or Password" is returned.
User.java (User Model)
A basic class representing a user.

username: Stores the username.
password: Stores the password.
Constructor: Initializes username and password.
Getter and Setter methods for username and password.
Screenshots:
(Screenshots provided in the original document would be inserted here, showing the initial login page, validation messages, locked account message, and success message.)
