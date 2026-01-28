# Welcome App

A simple full-stack application with Next.js frontend and Node.js backend, displaying content from a static JSON file.

## Project Structure

- **backend/** - Node.js Express API server
- **frontend/** - Next.js application

## Setup Instructions

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the server:
   ```bash
   npm run dev
   ```
   
   The backend will run on `http://localhost:3001`

### Frontend Setup

1. Open a new terminal and navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```
   
   The frontend will run on `http://localhost:3000`

## Usage

1. Start the backend server first (port 3001)
2. Start the frontend application (port 3000)
3. Open your browser to `http://localhost:3000`
4. You should see the welcome message loaded from the backend API

## Customization

### Changing the Content

Edit `backend/data/content.json` to modify the welcome message and features displayed on the page.

### Future Database Integration

The current setup uses a static JSON file. To swap it for a database:

1. Install your database driver (e.g., `mongodb`, `pg`, `mysql2`)
2. Update `backend/server.js` to connect to your database
3. Replace the file reading logic in the `/api/welcome` endpoint with database queries
4. The frontend code requires no changes!

## Tech Stack

- **Frontend:** Next.js 14 (React 18)
- **Backend:** Node.js with Express
- **Content:** Static JSON file
