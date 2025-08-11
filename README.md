# Job Portal Project (Full-Stack MERN)

## Table of Contents
1. [Project Overview](#project-overview)
2. [Technologies Used](#technologies-used)
3. [Features](#features)
4. [Installation](#installation)
5. [Usage](#usage)
6. [API Documentation](#api-documentation)
7. [Folder Structure](#folder-structure)
8. [Contributing](#contributing)
9. [License](#license)

## Project Overview
The **Job Portal** is a full-stack web application that connects job seekers with employers. Built using the **MERN Stack** (MongoDB, Express, React, Node.js), the platform allows job seekers to create profiles, search for jobs, and apply to job listings. Employers can post job vacancies, review applicants, and manage their job listings. The portal supports user authentication, provides an intuitive interface, and includes features such as job alerts, profile management, and an admin dashboard.

## Technologies Used
- **Frontend**: React.js, Redux (for state management), React Router, Bootstrap
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Token)
- **Other**: CSS, HTML5

## Features
- **User Authentication**: Job seekers and employers can sign up, log in, and manage their accounts with JWT-based authentication.
- **Job Seekers**:
  - Create and update personal profiles with work experience and skills.
  - Browse and search for job opportunities based on category, location, salary, and more.
  - Apply for jobs and track application status.
- **Employers**:
  - Post job listings with detailed descriptions.
  - View and manage applications from job seekers.
  - Edit or delete job postings.
- **Admin Dashboard**: Admin can manage users, job postings, and monitor site activity.
- **Job Alerts**: Notify job seekers about new job openings based on preferences.
- **Responsive Design**: Optimized for mobile and desktop views.

## Installation

### Prerequisites
- **Node.js**: [Download Node.js](https://nodejs.org/)
- **MongoDB**: You can use a local MongoDB instance or use [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) for a cloud-based database.

### Steps to Run the Application Locally

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ps2203/Job-Portal.git
````

2. **Install Backend Dependencies**:

   * Navigate to the backend folder and install the required dependencies:

     ```bash
     cd job-portal-mern/backend
     npm install
     ```

3. **Install Frontend Dependencies**:

   * Navigate to the frontend folder and install the required dependencies:

     ```bash
     cd ../frontend
     npm install
     ```

4. **Set Up MongoDB**:

   * If you're using **MongoDB Atlas**, create a cluster and get the connection string. Update the `backend/config/db.js` file with your MongoDB connection string.
   * If you're using a local MongoDB instance, ensure it is running and update the `db.js` file accordingly.

5. **Run the Application**:

   * Run the backend server:

     ```bash
     cd ../backend
     npm run dev
     ```
   * Run the frontend server:

     ```bash
     cd ../frontend
     npm start
     ```

6. **Access the Application**:
   Open your browser and go to `http://localhost:3000` to access the Job Portal.

## Usage

* Job seekers can register, log in, update their profiles, and apply to job listings.
* Employers can log in, post job vacancies, and review applications.
* Admin can manage users and job listings via the admin dashboard.

## API Documentation

The backend API provides the following routes:

### User Authentication

* **POST /api/users/register**: Register a new user.
* **POST /api/users/login**: Log in to an existing account.

### Job Listings

* **GET /api/jobs**: Fetch all available job listings.
* **POST /api/jobs**: Post a new job listing (Employer/Admin only).
* **GET /api/jobs/\:id**: Fetch a specific job listing.
* **PUT /api/jobs/\:id**: Update a job listing (Employer/Admin only).
* **DELETE /api/jobs/\:id**: Delete a job listing (Employer/Admin only).

### User Profiles

* **GET /api/profiles**: Fetch the profile of the logged-in user.
* **PUT /api/profiles**: Update the logged-in user's profile.

### Applications

* **POST /api/applications**: Apply to a job.
* **GET /api/applications**: Get all applications for a job (Employer only).

## Folder Structure

```
/job-portal-mern
|-- /backend
|   |-- /config         # Configuration files (e.g., database setup)
|   |-- /controllers    # Controllers handling business logic
|   |-- /models         # MongoDB models (e.g., Job, User)
|   |-- /routes         # Express routes (e.g., user, job)
|   |-- /middleware     # Authentication and validation middleware
|   |-- server.js       # Backend server entry point
|
|-- /frontend
|   |-- /src
|   |   |-- /components  # React components (e.g., JobList, Profile)
|   |   |-- /redux       # Redux state management (for cart, authentication, etc.)
|   |   |-- /screens     # Screens (e.g., Home, Login, JobDetail)
|   |   |-- App.js       # Main React component
|
|-- package.json        # Backend dependencies
|-- .env                # Environment variables (e.g., MongoDB URI, JWT secret)
```

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```

### Key Sections:
1. **Project Overview** - Briefly explains the purpose and features of the Job Portal.
2. **Technologies Used** - Lists all technologies and tools used to build the project.
3. **Features** - Highlights the functionalities of the portal, including what job seekers, employers, and admins can do.
4. **Installation** - Step-by-step guide for setting up the project locally.
5. **API Documentation** - Describes the various API endpoints used by the frontend and backend.
6. **Folder Structure** - Shows the layout of the project files for better organization.
7. **Contributing** - Instructions for other developers to contribute to the project.
8. **License** - Licensing details for the project.



