# react-blog
A react/node.js blog-app with MySql database
# React Blog App

A full-stack blogging application built with **React**, **Express.js**, and **MySQL** that allows users to create, edit, delete, and view blog posts.

---

## Features

- **User Authentication**: Register and login functionality.
- **Create Blog Posts**: Users can write articles with text, images, or videos.
- **Edit and Delete Posts**: Users can manage their own posts.
## Project Structure

The project consists of two main parts:

1. **Frontend**:
   - Built with React.
   - Contains pages such as Home, Login, Register, Write, and Single Post View.
   - Uses React Router for navigation.

2. **Backend**:
   - Built with Express.js.
   - Handles user authentication, posts management, and file uploads.
   - Connects to a MySQL database.

---

## Setup Instructions

### Prerequisites

- Node.js installed on your system.
- MySQL database setup.
- Git for version control.

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/react-blog.git
   cd react-blog
   ```

2. **Install dependencies**:
   - Navigate to the `frontend` directory:
     ```bash
     cd frontend
     npm install
     ```
   - Navigate to the `backend-api` directory:
     ```bash
     cd ../backend-api
     npm install
     ```

3. **Set up the database**:
   - Create a MySQL database.
   - Run the migrations to create tables:
     ```bash
     npx knex migrate:latest --knexfile knexfile.cjs
     ```
   - (Optional) Seed the database with dummy posts:
     ```bash
     npx knex seed:run --knexfile knexfile.cjs
     ```

4. **Configure environment variables**:
   - Create a `.env` file in the `backend-api` directory with the following content:
     ```env
     DB_HOST=your_database_host
     DB_USER=your_database_user
     DB_PASSWORD=your_database_password
     DB_NAME=your_database_name
     JWT_SECRET=your_jwt_secret
     ```

5. **Start the backend server**:
   ```bash
   cd backend-api
   npm run start
   ```

6. **Start the frontend**:
   ```bash
   cd ../frontend
   npm start
   ```

7. **Access the application**:
   - Open your browser and navigate to: `http://localhost:300

## Technologies Used

- **Frontend**: React, React Router, Axios, SCSS.
- **Backend**: Node.js, Express.js, MySQL, Knex.js.
- **Authentication**: JSON Web Tokens (JWT).
- **File Uploads**: Multer.



