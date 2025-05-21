# User Register & Login System

A simple web application for user registration and login with a modern UI. The frontend is built with HTML, CSS, and JavaScript, and communicates with a backend API for authentication.

## Features

- User registration with name, email, and password
- User login with email and password
- Toggle between registration and login forms
- Responsive, card-style UI
- Stores authentication token in local storage on successful login

## Folder Structure

```
user_register/
├── backend/         # Your backend code (API endpoints)
├── frontend/
│   ├── register.html
│   ├── style.css
│   └── script.js
```

## Getting Started

### Prerequisites

- Node.js (for backend)
- A modern web browser

### Environment Variables

The backend requires certain environment variables to be set. Create a `.env` file in your `backend` directory with the following example content:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
```

- `PORT`: The port your backend server will run on (default: 5000).
- `MONGO_URI`: MongoDB connection string.
- `JWT_SECRET`: Secret key for signing JWT tokens.

> **Note:** Adjust variable names as needed to match your backend implementation.

### Setup

1. **Clone the repository:**
   ```
   git clone <your-repo-url>
   ```

2. **Backend:**
   - Navigate to the `backend` folder.
   - Create a `.env` file as described above.
   - Install dependencies and start your backend server (see your backend's README or main file for details).
   - Ensure your backend runs on `http://localhost:5000` and exposes `/api/register` and `/api/login` endpoints.

3. **Frontend:**
   - Open `frontend/register.html` in your browser.

## Usage

- Click **Register** to create a new account.
- Click **Login** to sign in with your credentials.
- On successful login, you will be redirected to `dashboard.html` (create this page as needed).

## Customization

- Edit `style.css` to change the look and feel.
- Update API URLs in `script.js` if your backend runs on a different address.

## Troubleshooting

- If you see CORS errors, ensure your backend allows cross-origin requests.
- Make sure the backend server is running before using the frontend.

## License

This project is for educational purposes.