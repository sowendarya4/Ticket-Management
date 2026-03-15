# Mini Customer Support Ticket System

A full-stack ticket management system with real-time updates and email notifications.

## Tech Stack

### Backend
- **Express.js** (Node.js framework)
- **TypeScript**
- **Prisma ORM** (SQLite)
- **JWT** (Authentication)
- **Socket.io** (Real-time updates)
- **Nodemailer** (Email notifications)
- **Zod** (Validation)
- **Axios** (API requests)

### Frontend
- **React** (Vite)
- **TypeScript**
- **Tailwind CSS** (UI styling)
- **Lucide-React** (Icons)
- **Socket.io-client** (Real-time integration)
- **Axios** (API communication)

## Features

- **User Authentication**: Secure registration and login with password hashing and JWT.
- **Ticket Management (CRUD)**: Create, view, update status (Open/Closed), and delete tickets.
- **Real-Time Updates**: Instant UI updates when tickets are created, updated, or deleted using WebSockets.
- **Email Notifications**: Automatically send emails when a ticket is created or closed.
- **Third-Party API Integration**: Fetches and displays data from a public REST API in the dashboard.
- **Responsive UI**: Modern dashboard built with Tailwind CSS.

## Getting Started

### Prerequisites
- Node.js (v18+)
- npm

### Installation

1.  **Clone the repository**:
    ```bash
    git clone <repository-url>
    cd ticket-management
    ```

2.  **Setup Backend**:
    ```bash
    cd backend
    npm install
    # Generate Prisma Client and SQLite database
    npx prisma db push
    npx prisma generate
    # Create .env file with necessary variables
    ```

3.  **Setup Frontend**:
    ```bash
    cd ../frontend
    npm install
    ```

### Running the App

1.  **Start Backend Server**:
    ```bash
    cd backend
    npm run dev
    ```
    The backend will run on `http://localhost:5000`.

2.  **Start Frontend Dev Server**:
    ```bash
    cd frontend
    npm run dev
    ```
    The frontend will run on `http://localhost:5173` (or similar).

## API Documentation
A Postman collection is included in the root directory: `postman_collection.json`.

## Folder Structure
- `backend/`: Express server, Prisma schema, and API routes.
- `frontend/`: React application, components, and services.
- `prisma/`: Database migrations and schema.
