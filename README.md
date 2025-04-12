# Resume Building System

An Online resume building system with unique and ATS-friendly features, built with modern web technologies.

## Features

- 📚 Multiple ATS Template Selection
- 👥 User Authentication and Authorization
- 📱 Responsive Web Interface
- 📖 Export In Multiple Formats(PDF, DOCX, HTML)
- 📋 Profile Management
- 📁 Multiple Data-entry Feature
- ⚙️ Resume Preview and Layout Management 

## Tech Stack

### Backend
- Node.js with Express
- MongoDB with Mongoose
- JWT Authentication
- Nodemailer for emails

### Frontend
- React 18 with TypeScript
- Vite as build tool
- Material UI & Radix UI components
- TailwindCSS for styling
- React Router for navigation

## Prerequisites

- Node.js (v16 or higher)
- MongoDB
- npm or yarn
- SMTP server (for emails)

## Installation

1. Clone the repository
```bash
git clone [repository-url]
cd online_resume_builder
```

2. Install backend dependencies
```bash
cd backend
npm install
```

3. Install frontend dependencies
```bash
cd ../frontend
npm install
```

4. Set up environment variables
   - Create `.env` in the backend directory with:
     ```
     MONGODB_URI=your_mongodb_uri
     JWT_SECRET=your_jwt_secret
     GMAIL_USER=your_smtp_user
     GMAIL_APP_PASSWORD=your_smtp_password
     ```

## Running the Application

1. Start the backend server
```bash
cd backend
npm run start
```

2. Start the frontend development server
```bash
cd frontend
npm run dev
```

The application will be available at `http://localhost:5173` (frontend) and `http://localhost:3000` (backend API).

## Testing

### Backend Tests
```bash
cd backend
npm test
```

### Frontend Tests
```bash
cd frontend
npm test
```

## Project Structure

- `backend/` - Express server and Api
  - `controllers/` - Request handlers
  - `models/` - Database models
  - `routes/` - API routes
  - `middleware/` - Custom middleware
  - `services/` - Business logic
  - `utils/` - Helper functions

- `frontend/` - React application
  - `src/components/` - Reusable UI components
  - `src/pages/` - Page components
  - `src/services/` - API integration
  - `src/utils/` - Helper functions

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

MIT License


<p align="center">
  <img src="https://github.com/user-attachments/assets/eb7e9ae0-a7d9-434f-b520-297321d4cccf" width="45%" />
  <img src="https://github.com/user-attachments/assets/cbe6e83f-09c9-444c-afd1-9de8b0d3eaac" width="45%" />
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/eaeb8331-7190-4f4b-9c19-bfae4be16dc7" width="45%" />
  <img src="https://github.com/user-attachments/assets/51d98ac3-bdcd-4b75-9827-6e840be36649" width="45%" />
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/f21b3d76-175c-480c-a61e-de1c88b87b1a" width="45%" />
</p>
