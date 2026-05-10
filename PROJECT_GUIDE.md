# Cybersecurity System - Diploma Level Project

## 📋 Project Overview

This is a simple cybersecurity system designed for diploma-level students. It demonstrates three basic cybersecurity features:

1. **Login System** - User authentication with email and password
2. **Password Strength Checker** - Evaluates password security and provides suggestions
3. **Phishing Detection Tool** - Analyzes URLs for potential phishing risks

---

## 🛠️ Technologies Used

### Frontend
- **React** - JavaScript library for building user interfaces
- **HTML5** - Markup language
- **CSS3** - Styling with modern gradients and responsive design
- **Babel** - JavaScript compiler (for JSX in browser)

### Backend
- **Node.js** - JavaScript runtime environment
- **Express** - Web framework for Node.js
- **CORS** - Cross-origin resource sharing middleware
- **Body Parser** - Middleware to parse JSON request bodies

---

## 📁 Project Structure

```
oscar/
├── backend/
│   ├── index.js          # Backend server with all API endpoints
│   └── package.json      # Backend dependencies
├── frontend/
│   ├── index.html        # Main HTML file
│   ├── app.js            # React application (all components)
│   ├── styles.css        # Complete styling
│   └── package.json      # Frontend configuration
├── PROJECT_GUIDE.md      # This file (project documentation)
└── README.md             # Quick start guide
```

---

## 🚀 How to Run the Project

### Step 1: Install Dependencies

First, open two terminal windows (one for backend, one for frontend).

**Backend Terminal:**
```bash
cd backend
npm install
```

**Frontend Terminal:**
```bash
cd frontend
npm install
```

### Step 2: Start the Backend Server

In the backend terminal:
```bash
npm start
```

You should see:
```
========================================
Cybersecurity System Backend
Server running on http://localhost:5000
========================================
```

### Step 3: Start the Frontend

In the frontend terminal:
```bash
npm start
```

This will start a local server. Open your browser and go to the URL shown (usually `http://localhost:3000` or similar).

---

## 🎯 Features Explained

### 1. Login System

**What it does:**
- Allows users to enter email and password
- Verifies credentials against a dummy user database
- Shows success or error messages

**Test Credentials:**
- Email: `student@diploma.edu`
- Password: `SecurePass123!`

**Backend Code Location:** `backend/index.js` lines 34-59

---

### 2. Password Strength Checker

**What it does:**
- Evaluates password strength based on 5 criteria:
  1. Minimum 8 characters
  2. Contains uppercase letter (A-Z)
  3. Contains lowercase letter (a-z)
  4. Contains number (0-9)
  5. Contains special character (!@#$%^&*)

- Displays:
  - Strength level (Too Short → Weak → Medium → Strong → Very Strong)
  - Score (0-5)
  - Visual strength bar with colors
  - Suggestions for improvement

**Strength Levels:**
- Too Short: < 6 characters
- Weak: 0-2 points
- Medium: 3 points
- Strong: 4 points
- Very Strong: 5 points

**Backend Code Location:** `backend/index.js` lines 64-145

---

### 3. Phishing Detection Tool

**What it does:**
- Analyzes URLs for 3 common phishing indicators:
  1. Missing HTTPS (not secure connection)
  2. Suspicious keywords (free, login, verify, bank, etc.)
  3. Too many hyphens (> 3)

- Displays:
  - Safe/Suspicious verdict
  - List of specific risks found

**Suspicious Keywords Checked:**
```
free, login, verify, update, bank, secure,
account, password, signin, confirm, wallet,
paypal, facebook, google, apple, microsoft
```

**Backend Code Location:** `backend/index.js` lines 150-207

---

## 💡 How to Explain During Project Defense

### Opening Statement
> "Good morning/afternoon. Today I'll be presenting my diploma project: a Simple Cybersecurity System. This project demonstrates three fundamental cybersecurity concepts: user authentication, password security, and phishing detection."

---

### Explaining the Login System
> "First, let's look at the Login System. This feature shows how user authentication works. I've created a dummy user database with one test account. When the user enters their email and password, the frontend sends a request to the backend API at `/api/login`. The backend checks if the credentials match, and sends back a success or error message."

---

### Explaining the Password Strength Checker
> "Next is the Password Strength Checker. This teaches users how to create secure passwords. The system evaluates passwords using 5 criteria: length, uppercase, lowercase, numbers, and special characters. Each criterion gives 1 point, for a maximum of 5 points. Based on the score, it shows a strength level and helpful suggestions. For example, if a password is missing an uppercase letter, it will tell the user to add one."

---

### Explaining the Phishing Detection Tool
> "Third is the Phishing Detection Tool. Phishing is when attackers create fake websites to steal information. My tool checks URLs for red flags: first, does it use HTTPS? HTTPS encrypts data between the browser and server. Second, does it contain suspicious keywords like 'login' or 'verify' that phishers often use? Third, does it have too many hyphens, which is common in fake URLs? The tool then tells the user if the link appears safe or suspicious."

---

### Technology Stack Explanation
> "For the frontend, I used React because it makes it easy to create interactive user interfaces with components. The backend uses Node.js and Express, which let me build a simple API server quickly. All communication between frontend and backend uses JSON format."

---

### Closing
> "In conclusion, this project demonstrates basic but important cybersecurity concepts in a practical way. It's simple enough for beginners to understand, but shows real-world applications of security principles. Thank you for your attention, and I'm ready for any questions."

---

## 🔧 Customization Tips

### Adding More Users
Edit `backend/index.js` lines 22-29:
```javascript
const USERS = [
  {
    id: 1,
    email: 'student@diploma.edu',
    password: 'SecurePass123!',
    name: 'Diploma Student'
  },
  // Add more users here
  {
    id: 2,
    email: 'another@example.com',
    password: 'AnotherPass456!',
    name: 'Another User'
  }
];
```

### Changing Password Criteria
Edit `backend/index.js` lines 91-119 in the password checker function.

### Adding More Phishing Checks
Edit `backend/index.js` lines 165-192 in the phishing detection function.

---

## 📚 Key Cybersecurity Concepts Demonstrated

1. **User Authentication** - Verifying user identity
2. **Password Security** - Best practices for strong passwords
3. **HTTPS Importance** - Secure communication
4. **Phishing Awareness** - Recognizing suspicious URLs
5. **Client-Server Architecture** - Frontend vs Backend separation
6. **API Communication** - RESTful API endpoints
7. **Input Validation** - Checking user input
8. **Error Handling** - Gracefully handling errors

---

## ⚠️ Important Notes

- This is an **educational project** only
- Passwords are stored in plain text (for simplicity) - in real projects, use password hashing (bcrypt)
- No database (MongoDB) is used - uses in-memory dummy data
- Phishing detection is basic - real systems use more advanced techniques
- Always keep security in mind when building real applications

---

## 🎓 Ready for Presentation!

You now have:
✅ Complete working code
✅ Beautiful user interface
✅ Detailed documentation
✅ Presentation script
✅ Customization options

Good luck with your project defense! 🎉
