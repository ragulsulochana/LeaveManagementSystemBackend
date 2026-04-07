# Leave Management System

A full-stack leave management application with role-based access control built with React (frontend) and Node.js/Express (backend).

## Features

### Authentication
- Login/Signup with role selection (Student, Staff, HOD, Principal)
- JWT-based authentication
- Password hashing with bcrypt

### Role-Based Access

#### Student
- Dashboard with leave statistics
- Apply for leave with date range, reason, and proof upload
- View leave status with approval timeline
- Profile management

#### Staff
- Review pending leave requests
- Approve/Reject student applications
- View approved and rejected requests

#### HOD (Head of Department)
- Review staff-approved requests
- Department overview statistics
- Approve/Reject applications

#### Principal
- Final approval/rejection of HOD-approved requests
- Add new HOD profiles
- System-wide statistics

## Tech Stack

### Frontend
- React 19
- React Router for navigation
- Material-UI for components
- Axios for API calls
- date-fns for date formatting

### Backend
- Node.js
- Express.js
- JWT for authentication
- bcryptjs for password hashing
- CORS for cross-origin requests

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd leave-management-system
   ```

2. **Backend Setup**
   ```bash
   cd backend
   npm install
   npm start
   ```
   The backend will run on http://localhost:5000

3. **Frontend Setup**
   ```bash
   cd my-react-app
   npm install
   npm run dev
   ```
   The frontend will run on http://localhost:5173

## Demo Credentials

Use password: `password` for all accounts

- **Student**: student@demo.com
- **Staff**: staff@demo.com
- **HOD**: hod@demo.com
- **Principal**: principal@demo.com

## API Endpoints

### Authentication
- `POST /api/auth/login` - User login
- `POST /api/auth/signup` - User registration

### Leaves
- `GET /api/leaves` - Get leaves based on user role
- `GET /api/leaves/user` - Get current user's leaves
- `POST /api/leaves` - Submit new leave request
- `PUT /api/leaves/:id/approve` - Approve leave
- `PUT /api/leaves/:id/reject` - Reject leave

## Project Structure

```
leave-management-system/
├── backend/
│   ├── server.js
│   └── package.json
├── my-react-app/
│   ├── src/
│   │   ├── components/
│   │   │   ├── auth/
│   │   │   ├── student/
│   │   │   ├── staff/
│   │   │   ├── hod/
│   │   │   └── principal/
│   │   ├── contexts/
│   │   └── ...
│   └── package.json
└── README.md
```

## Features Overview

- **Responsive Design**: Works on desktop and mobile
- **Material Design**: Modern UI with Material-UI components
- **Role-based Routing**: Different dashboards for each user type
- **Real-time Updates**: State management with React Context
- **Secure Authentication**: JWT tokens with protected routes
- **Approval Workflow**: Multi-stage approval process (Staff → HOD → Principal)

## Development

### Adding New Features
1. Update backend API endpoints in `backend/server.js`
2. Add frontend components in appropriate directories
3. Update routing in `App.jsx`
4. Test with different user roles

### Styling
- Uses Material-UI theme system
- Custom theme defined in `main.jsx`
- Consistent color scheme and typography

## License

This project is for educational purposes.