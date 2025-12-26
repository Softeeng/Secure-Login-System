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
```bash
https://github.com/Softeeng/Secure-Login-System
```

2. Run the application:
```bash
python secure_login.py
```

## Usage

# Registration
1. Select "Register" from the main menu
2. Enter username and email
3. Create a strong password (requirements enforced):
    - Minimum 8 characters
    - At least one uppercase letter
    - At least one lowercase letter
    - At least one number
4. Select role (Doctor or Patient)

# Login
1. Select "Login" from the main menu
2. Enter your username and password
3. Access role-specific dashboard

# Role-Based Features

**Doctor Dashboard:**
- Access patient records
- Manage appointments
- Write prescriptions
- View medical reports

**Patient Dashboard:**
- View personal medical records
- Book appointments
- View prescriptions
- Access test results

## Project Structure
```text
secure-login-system/    
├── secure_login.py     # Main application file
├── users.json          # User database (auto-generated, not tracked)
├── .gitignore          # Git ignore rules
└── README.md           # This file
```

## Security Implemenation

# Password Hashing
    # SHA-256 hashing with unique salt password + unique_salt ➡️ SHA-256 ➡️ stored_hash

# Authentication Flow
1. User enters credentials
2. System retrieves stored salt for username
3. Hashes provided password with stored salt
4. Compares hashes (constant-time comparison)
5. Grant access if hashes match

# Session Management 
- Tracks currently logged-in user
- Updates last login timestamp
- Maintains session until explicit logout

## Learning Objectives
This project helped me understand:
- Cryptographic password hashing (SHA-256)
- Salt generation and usage
- Role-based access control (RBAC)
- Session management
- Secure authentication flows
- Password strength validation

## Future Enhancements
**Planned Improvements:**
- Password reset functionality
- Account lockout after failed attempts
- Two-factor authentication (2FA)
- Password expiration policies
- Audit logging for security events
- Integration with other healthcare modules

## Roadmap Context
**Month 2 Goals:**
- ✅Secure Login System- Role-based access control
- ⌛Appointment Booking System (Next)

