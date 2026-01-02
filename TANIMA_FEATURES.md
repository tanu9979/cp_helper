# Algonauts CP Helper - Authentication & Mentor Features

## Overview
This project implements a comprehensive authentication system and mentor dashboard for competitive programming practice management.

## Features Implemented by Tanima

### Backend Authentication System
- **JWT-based Authentication**: Secure token-based authentication with HTTP-only cookies
- **Role-based Access Control**: Separate access levels for mentors and students
- **Enhanced Security**: Rate limiting, password validation, and session management
- **User Management**: Registration, login, logout, and profile management

### Mentor Dashboard Features
- **Group Management**: Create and manage student groups
- **Problem Assignment**: Assign problems and track student progress
- **Contest Creation**: Create both group-specific and global contests
- **Analytics**: Comprehensive statistics and progress tracking
- **Student Management**: Add students to groups and monitor their performance

### Frontend Components
- **Authentication Pages**: Login and registration with role selection
- **Mentor Dashboard**: Complete interface for mentor operations
- **Protected Routes**: Role-based route protection
- **State Management**: Global authentication state with React Context

## Security Features
- Password hashing with bcrypt
- JWT token validation
- Rate limiting on API endpoints
- Input validation and sanitization
- Session timeout management

## API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout
- `GET /api/auth/me` - Get current user profile

### Mentor Operations
- `POST /api/mentor/create-group` - Create new group
- `GET /api/mentor/groups` - Get mentor's groups
- `POST /api/mentor/add-students/:groupId` - Add students to group
- `POST /api/mentor/create-contest/:groupId` - Create contest
- `GET /api/mentor/group-stats/:groupId` - Get group statistics

## Technologies Used
- **Backend**: Node.js, Express.js, MongoDB, JWT
- **Frontend**: React, React Router, Context API
- **Security**: bcrypt, express-rate-limit, CORS
- **Database**: MongoDB with Mongoose ODM

## Installation & Setup
1. Clone the repository
2. Install dependencies: `npm install` in both backend and frontend directories
3. Set up environment variables in backend/.env
4. Start MongoDB service
5. Run backend: `npm start`
6. Run frontend: `npm run dev`

## Author
**Tanima Samanta** (tanu9979)
- Email: tanimasamanta97@gmail.com
- GitHub: https://github.com/tanu9979