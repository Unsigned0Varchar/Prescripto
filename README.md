# Prescripto - Doctor Appointment Booking System

Prescripto is a comprehensive full-stack application for booking doctor appointments. It includes a user-facing frontend for patients to browse doctors and book appointments, an admin panel for managing doctors and appointments, and a robust backend API.

## 🚀 Tech Stack

### Backend
- **Node.js** & **Express.js**: RESTful API server.
- **MongoDB** & **Mongoose**: Database and object modeling.
- **Cloudinary**: Image storage and management.
- **Razorpay**: Payment gateway integrations.
- **JWT**: JSON Web Tokens for authentication.
- **Multer**: Middleware for handling file uploads.

### Frontend (User & Admin)
- **React.js**: UI library.
- **Vite**: Fast build tool and development server.
- **Tailwind CSS**: Utility-first CSS framework for styling.
- **Axios**: HTTP client for API requests.
- **React Router**: Client-side routing.
- **React Toastify**: Notifications.

## 📂 Project Structure

```
prescripto-full-stack/
├── admin/          # Admin panel frontend (React + Vite)
├── backend/        # Backend API (Node.js + Express)
└── frontend/       # User-facing frontend (React + Vite)
```

## 🛠️ Installation & Setup

### Prerequisites
- Node.js installed on your machine.
- MongoDB database (local or Atlas).
- Cloudinary account.
- Stripe/Razorpay accounts (for payments).

### 1. Backend Setup

Navigate to the backend directory:
```bash
cd backend
```

Install dependencies:
```bash
npm install
```

Create a `.env` file in the `backend` directory with the following variables:
```env
PORT=4000
MONGODB_URI=your_mongodb_connection_string
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
```

Start the server:
```bash
npm start
# or for development with nodemon
npm run server
```

### 2. Frontend Setup

Navigate to the frontend directory:
```bash
cd frontend
```

Install dependencies:
```bash
npm install
```

Start the development server:
```bash
npm run dev
```

### 3. Admin Panel Setup

Navigate to the admin directory:
```bash
cd admin
```

Install dependencies:
```bash
npm install
```

Start the development server:
```bash
npm run dev
```

## 🔌 API Endpoints

The backend exposes the following main route groups:
- `/api/user`: User authentication and profile management.
- `/api/doctor`: Doctor-related operations.
- `/api/admin`: Admin dashboard operations.

## ✨ Features

- **Doctor Browsing**: Users can view a list of doctors and filter by specialization.
- **Appointment Booking**: specific time slots can be booked.
- **Admin Dashboard**: Manage doctors, view all appointments.
- **Doctor Dashboard**: Doctors can log in to view their appointments.
- **Secure Payments**: Integrated with Stripe and Razorpay.
- **Responsive Design**: Works on mobile and desktop.
