# Vehicle Management System

## Project Overview

The Vehicle Management System is a comprehensive web application designed to streamline vehicle servicing and transportation operations. The application provides a centralized platform for customers, mechanics, drivers, and administrators to manage vehicle-related tasks efficiently.

## Key Features and Security Objectives

### Major Functionalities
- User Registration and Authentication
- Service Request Management
- Task Assignment for Mechanics
- Route Management for Drivers
- Admin Dashboard and Control Panel
- Feedback and Communication System

### Security Objectives
- Robust User Authentication
- Role-Based Access Control
- Input Validation and Sanitization
- Protection Against Common Web Vulnerabilities
- Secure Session Management
- Data Privacy and Integrity

## Project Structure


## Setup and Installation

### Prerequisites
- Python 3.8+
- pip
- virtualenv (recommended)

### Installation Steps
1. Clone the repository
```bash
git clone https://github.com/yourusername/vehicle-management-system.git
cd vehicle-management-system    
```

2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Configure environment variables
- Create a .env file in the project root
- Add necessary configuration (SECRET_KEY, database settings)

5. Run database migrations
```bash
python manage.py makemigrations
python manage.py migrate
```

6. Create superuser
```bash
python manage.py createsuperuser
```

7. Run the development server
```bash
python manage.py runserver
```

### Usage Guidelines
1. User Registration
- Navigate to the registration page
- Choose user type (Customer, Mechanic, Driver)
- Fill in required details
- Submit registration

2. Login
- Enter credentials on the login page
- Select appropriate user role
- Access role-specific dashboard

3. Key Features by Role
- Customers: Submit service requests, track status
- Mechanics: View assigned tasks, update repair status
- Drivers: View routes, update route status
- Administrators: Manage users, assign tasks, generate reports

### Security Improvements
1. Authentication
- Implemented Django's built-in authentication system
- Multi-layer password validation
- Role-based access control

2. Input Security
- Server-side input validation
- Protection against SQL injection
- CSRF token implementation
- XSS prevention

3. Network Security
- HTTPS enforcement
- Secure cookie settings
- Content Security Policy
- Strict host validation

4. Session Management
- Secure session handling
- Session timeout
- Logout mechanism with session destruction

### Security Testing
1. Tools Used
- Django built-in security middleware
- Bandit (Python security linter)
- OWASP ZAP (Vulnerability scanner)

2. Testing Approach
- Static code analysis
- Penetration testing
- Input validation checks
- Authentication scenario testing

### Contributions
1. Technologies
* Backend: Django (Python)
* Frontend: HTML, CSS, JavaScript
* Database: MySQL
