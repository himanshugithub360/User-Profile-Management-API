# User Profile Management API

This is a RESTful API for managing user profiles with authentication using JWT. Users can register, log in, retrieve, and update their profiles securely.

## Features

- User registration and login with JWT authentication
- Profile retrieval and update
- Secure password hashing using bcrypt
- Protected routes (users can only access their own profiles)
- MongoDB as the database
- Error handling

## Tech Stack

- Backend: Node.js, Express.js
- Database: MongoDB
- Authentication: JWT

## Installation

### 1. Clone the repository

\`\`\`sh
git clone https://github.com/himanshugithub360/User-Profile-Management-API.git
cd User-Profile-Management-API
\`\`\`

### 2. Install dependencies

\`\`\`sh
npm install
\`\`\`

### 3. Configure Environment Variables

Create a \`.env\` file in the root directory and add the following:

\`\`\`
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
PORT=5000
\`\`\`

### 4. Run the server

#### Development Mode (with auto-restart)

\`\`\`sh
npm run dev
\`\`\`

#### Production Mode

\`\`\`sh
npm start
\`\`\`

## API Endpoints

### **Authentication Routes**

- **Register User**: \`POST /api/auth/register\`
- **Login User**: \`POST /api/auth/login\`

### **User Profile Routes**

- **Get Profile**: \`GET /api/users/profile\` *(Auth Required)*
- **Update Profile**: \`PUT /api/users/profile\` *(Auth Required)*

## Testing with Postman

1. Import the provided Postman collection (if available).
2. Use the \`POST /api/auth/register\` endpoint to create a user.
3. Log in via \`POST /api/auth/login\` to get a token.
4. Add the token in the Authorization header to access protected routes.

## Deployment

To deploy, use platforms like:

- **Heroku**
- **Render**
- **Vercel**
- **DigitalOcean**




