# Todo App

A simple full‑stack Todo application built with React, Vite, Express, and MongoDB.

## Features
- Create, read, update, delete todos
- Responsive UI with a modern blue theme
- Loading states and error handling
- CORS enabled, environment‑based configuration

## Prerequisites
- Node.js v20+ (recommended)
- MongoDB instance (local or Atlas)

## Setup

### Backend
bash
cd backend
npm install
cp .env.example .env
# Edit .env with your MongoDB URI
npm start


### Frontend
bash
cd frontend
npm install
npm run dev


The frontend will be served at `http://localhost:5173` by default. It will communicate with the backend at `http://localhost:5000` (or the URL defined in `VITE_API_URL`).

## Environment Variables

### Backend (.env)
- `PORT` – Port for Express server (default: 5000)
- `MONGO_URI` – MongoDB connection string

### Frontend (.env)
- `VITE_API_URL` – Base URL for the backend API (default: `http://localhost:5000`)

## Project Structure

frontend/
  src/
    App.jsx
    App.css
    main.jsx
  index.html
  package.json
backend/
  server.js
  package.json
  .env.example
README.md


## License
MIT