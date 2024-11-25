
# Project Overview
It is my individual project,
StudyHub is an online educational platform that facilitates seamless interaction among students, teachers, and administrators. The platform incorporates a robust role-based login system, user authentication, and authorization to ensure secure and personalized access for each type of user.

# Deployed Link : 
https://studyhub123.netlify.app/

# Features

## General Features
- **User Authentication:** Secure login system using encrypted credentials.
- **Role-Based Authorization:** Different functionalities based on user roles (Student, Teacher, Admin).
- **Responsive Design:** The website is accessible across various devices, including desktops, tablets, and mobile phones.
- **Course Management:** Access to a comprehensive library of courses tailored for students and managed by teachers and admins.

## Role-Based Functionality
   **1. Student Role:**
  - Can go through with courses and its description.
  - Access to enrolled courses with progress tracking.
  - Ability to explore the course library and enroll in available  courses.
  
  **2. Teacher Role:**
  - Create and manage courses, including uploading study materials and assignments.
  - Monitor student progress and provide feedback on assignments.
  
  **3. Admin Role** (Right now Admin not able to login from frontend, it work only on backend, other two student, teacher are in frontend):
  - Manage user accounts for students and teachers (add, remove, or update profiles).
  - Can Add New Courses.
  - Oversee platform activities and generate reports.

## Tech Stack
 - **Frontend:** React.js for building dynamic and interactive user interfaces.
 - **Backend:** Node.js and Express.js for handling server-side logic and API integration.
 - **Database:** MongoDB for storing user data, course information, and progress tracking.
 - **Authentication:** JSON Web Tokens (JWT) for user authentication and session management.

 ## Authentication and Authorization
**Authentication:**
- Users must register and log in to access the platform.
Passwords are hashed using a secure algorithm for storage.
- Login credentials are verified against the database to grant access.
**Authorization:**
- After successful login, a JWT token is issued to the user for session validation.
- The platform checks user roles (student, teacher, admin) to authorize access to specific routes and resources.
- Unauthorized access to restricted features is prevented, ensuring data security.
# Installation and Setup

## 1. Clone the repository:

```bash
  git clone https://github.com/your-username/studyhub.git  
  cd studyhub
```


## 2. Install dependencies for the Frontend:

```bash
   cd frontend  
   npm install
```

## 3. Install dependencies for the Backend:

```bash
   cd backend  
   npm install & other dependencies.
```

## 4. Set up the environment variables:

- Create a .env file in the root directory.
- Add the following variables:

```bash
    MONGO_URI=<your_mongo_database_url>  
    PORT = ""
    
    MAIL_HOST = ""
    MAIL_USER = ""
    MAIL_PASS = ""

    JWT_SECRET = ""
    FOLDER_NAME = ""

    RAZORPAY_KEY = ""
    RAZORPAY_SECRET = ""

    CLOUD_NAME = ""
    API_KEY = ""
    API_SECRET = ""
```

## 5. Start the application: 
```bash
    npm start   
```

