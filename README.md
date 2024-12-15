# HotelHub

## Overview
This project demonstrates the creation of a full-stack hotel booking application using the **MERN stack** (MongoDB, Express, React, Node.js). The application allows users to search for hotels, reserve rooms, view dynamic pricing, and manage bookings. An admin dashboard is included to manage hotels and rooms.

---

## Features
- **User Features:**
  - Hotel search with filters for price, dates, and availability.
  - Dynamic updates for date and price changes.
  - User authentication for secure room reservations.
  - Ability to view detailed hotel information and calculate pricing.
- **Admin Features:**
  - Admin dashboard for managing hotels and rooms (CRUD operations).
  - Add, update, or delete hotel and room information seamlessly.
- **Advanced Search:**
  - Filters for price range, dates, and room availability.
  - Dynamic updates to exclude unavailable rooms for overlapping bookings.
- **Error Handling:**
  - Comprehensive error messages for users and developers.
  - Middleware for logging and managing API request issues.

---

## Technologies Used

### Frontend:
- **React**: For building the dynamic user interface.
- **React Router**: For navigation and routing within the app.
- **Redux (or Context API)**: For state management across components.
- **CSS/Styled-Components**: For responsive and aesthetic UI design.

### Backend:
- **Node.js**: For server-side scripting and backend logic.
- **Express.js**: For routing and creating RESTful APIs.
- **MongoDB**: For database storage of hotel, room, and booking data.
- **Mongoose**: For interacting with the MongoDB database.

### Authentication & Security:
- **JWT (JSON Web Tokens)**: For secure user authentication.
- **HTTP-only Cookies**: For storing authentication tokens securely.
- **Password Hashing**: To ensure secure user login and registration.

### Deployment:
- **MongoDB Atlas**: For cloud database hosting.
- **Heroku/Vercel**: For deploying the application.
- **Git/GitHub**: For version control and collaboration.

---

## Installation and Setup

### Prerequisites
- **Node.js** (v14 or above)
- **MongoDB Atlas** account for database setup
- **Git** installed on your system

### Steps
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```
2. **Install Dependencies:**
   ```bash
   npm install
   cd client
   npm install
   ```
3. **Environment Setup:**
   - Create a `.env` file in the root directory with the following variables:
     ```env
     PORT=5000
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_secret_key
     CLIENT_URL=http://localhost:3000
     ```
4. **Run the Application:**
   - Backend:
     ```bash
     npm run start
     ```
   - Frontend:
     ```bash
     cd client
     npm start
     ```
5. **Access the Application:**
   - Frontend: [http://localhost:3000](http://localhost:3000)
   - Backend: [http://localhost:5000](http://localhost:5000)

---

## Usage

### User Workflow:
1. Search for hotels by selecting destination, dates, and room options.
2. View search results dynamically updated based on filters (e.g., price range).
3. View detailed hotel information, calculate pricing, and make reservations.
4. Log in or sign up to reserve rooms securely.

### Admin Workflow:
1. Log in to the admin dashboard.
2. Add, update, or delete hotels and rooms via intuitive forms.
3. Manage all bookings and monitor data.

---

## Custom Hooks and State Management
- **Custom Hooks:**
  - `useFetch`: For handling API requests efficiently.
- **Context API:**
  - Centralized state management for global data access.

---

## Database Setup
- Hosted on **MongoDB Atlas**.
- Steps:
  1. Create a MongoDB Atlas cluster.
  2. Add your IP address to the network access list.
  3. Create collections for `users`, `hotels`, and `rooms`.

---

## Error Handling
- Middleware for handling API errors and logging issues.
- Custom error messages for seamless debugging and user guidance.

---

## Deployment
1. Prepare the environment by setting up `.env` variables for production.
2. Build the frontend:
   ```bash
   cd client
   npm run build
   ```
3. Deploy the backend and frontend using **Heroku** or **Vercel**.
