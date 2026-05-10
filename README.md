# 🔐 Cybersecurity System - Diploma Level Project

A simple, beginner-friendly cybersecurity demonstration project built with React, Node.js, and Express. Perfect for diploma-level presentations!

## ✨ Features

1. **Login System** - User authentication with email and password verification
2. **Password Strength Checker** - Evaluates password security with visual feedback and suggestions
3. **Phishing Detection Tool** - Analyzes URLs for potential phishing risks

## 🚀 Quick Start

### Prerequisites
- Node.js installed on your computer

### Installation & Setup

1. **Install Backend Dependencies**
   ```bash
   cd backend
   npm install
   ```

2. **Install Frontend Dependencies**
   ```bash
   cd ../frontend
   npm install
   ```

### Running the Application

**Terminal 1 - Backend:**
```bash
cd backend
npm start
```

**Terminal 2 - Frontend:**
```bash
cd frontend
npm start
```

Then open your browser and go to the URL shown in the frontend terminal!

## 🔑 Test Credentials

- **Email:** `student@diploma.edu`
- **Password:** `SecurePass123!`

## 📚 Documentation

For detailed explanations, presentation tips, and customization guides, see **[PROJECT_GUIDE.md](PROJECT_GUIDE.md)** - this includes everything you need for your project defense!

## 🛠️ Tech Stack

- **Frontend:** React, HTML5, CSS3
- **Backend:** Node.js, Express, CORS, Body Parser
- **Architecture:** RESTful API with client-server separation

## 📁 Project Structure

```
oscar/
├── backend/
│   ├── index.js          # Backend server with API endpoints
│   └── package.json      # Backend dependencies
├── frontend/
│   ├── index.html        # Main HTML file
│   ├── app.js            # React application
│   ├── styles.css        # Styling
│   └── package.json      # Frontend config
├── PROJECT_GUIDE.md      # Complete documentation & presentation guide
└── README.md             # This file
```

## 🎯 Features in Detail

### 1. Login System
- Simple email/password authentication
- Success/error messages with color coding
- Uses a dummy user database (easily extendable)

### 2. Password Strength Checker
- 5-point scoring system
- Visual strength bar with colors
- Strength levels: Too Short → Weak → Medium → Strong → Very Strong
- Personalized suggestions for improvement

### 3. Phishing Detection Tool
- Checks for HTTPS (secure connection)
- Scans for suspicious keywords
- Detects excessive hyphens
- Lists specific risks found

## 💡 Educational Purpose

This project is designed for **learning and demonstration** only. It intentionally keeps things simple to make cybersecurity concepts easy to understand and explain.

## 🎓 Ready for Your Diploma Defense!

Check out **[PROJECT_GUIDE.md](PROJECT_GUIDE.md)** for:
- Line-by-line code explanations
- Presentation talking points
- Customization tips
- Key cybersecurity concepts demonstrated

Good luck with your project! 🎉
