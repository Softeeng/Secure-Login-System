## Secure Login System ##
A role-based authentication system for healthcare applications, built with Python. Part of my [6-Month Healthcare IT learning journey](https://github.com/Softeeng/6-Month-Roadmap).

## Features

# 🔐Security Features
- **Password Hashing:** SHA-256 with unique salt for each user
- **Password Strength Validation:** Enforces strong password requirements
- **Secure Storage:** Passwords never stored in plain text
- **Session Management:** Track login status and last login time

# 👤User Management
- **User Registration:** Create new accounts with role assignment
- **User Login/Logout:** Secure authentication system
- **Role-Based Access Control:**
    - **Doctor:** Access to patient records, appointments, prescriptions
    - **Patient:** Access to personal medical records, appointment booking

# 📊User Profile
- **View profile information**
- **Track account creation date**
- **Monitor last login time**

## Requirements
- **Python 3.6 or higher**
- **No external dependencies (uses only standard library)**

## Installation
1. Clone this repository: