# 🚀 React URL Shortener Web App

A fully functional, responsive **React-based URL Shortener** application developed for the **Campus Hiring Frontend Evaluation**.  
This app allows users to shorten URLs, manage them with expiry times, track click statistics, and handle redirection – all with **client-side persistence** and **custom logging middleware**.

---

## 📌 Features

- 🔗 **URL Shortening** – Generate unique short links with optional custom shortcodes.  
- ⏳ **Expiry Handling** – Set a validity period for shortened URLs (default: 30 minutes).  
- 📊 **Statistics Dashboard** – Track usage history, including:
  - Total clicks per link  
  - Timestamp of each click  
  - Referrer & approximate location info  
- 🔄 **Redirection Support** – Visiting a short link redirects to the original URL.  
- 🛠 **Client-Side Persistence** – All data is stored locally using `localStorage`.  
- 🧩 **Reusable Logging Middleware** – Custom-built logging system used across API calls, components, hooks, and routes.  

---

## 🏗 Architecture & Design

- **Frontend Framework**: [React](https://react.dev/) – Modular, component-driven UI.  
- **Routing**: [react-router-dom](https://reactrouter.com/) – Client-side routing for shortener, redirect, and stats pages.  
- **UI Library**: [Material UI (MUI)](https://mui.com/) – Pre-styled, responsive UI components.  
- **Date Handling**: [Day.js](https://day.js.org/) – Manage expiry & timestamps.  
- **Shortcode Generation**: [Nanoid](https://github.com/ai/nanoid) – Generates unique, collision-resistant shortcodes.  
- **Persistence**: Browser `localStorage` – No backend required.  
- **Logging Middleware**: Custom-built, reusable package integrated throughout the app.  

### 📂 Project Structure
```
.
├── logging-middleware/      # Reusable logger package
├── frontend-test/           # React frontend application
│   ├── src/
│   │   ├── pages/           # ShortenerPage, StatsPage, RedirectPage
│   │   ├── components/      # Reusable UI components
│   │   ├── services/        # URL & storage utilities
│   │   ├── hooks/           # Custom React hooks
│   │   └── App.js
│   └── package.json
└── README.md
```

---

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/AbhishekSriv6387/2201640130004.git
   cd url-shortener-app
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run the development server**
   ```bash
   npm start
   ```

4. Open the app in your browser at 👉 [http://localhost:3000](http://localhost:3000)

---

## 📜 Usage Guide

1. Navigate to the **Shortener Page**  
   - Enter the original URL  
   - Optionally add an expiry time (in minutes)  
   - Optionally provide a custom shortcode  

2. View generated short links in the **results section** with expiry details.  

3. Access the **Statistics Page** to view:  
   - List of all shortened URLs  
   - Creation & expiry times  
   - Click history (timestamps, referrer, location).  

---

## 🔒 Assumptions

- Authentication is assumed (no login mechanism required for test).  
- Persistence is handled entirely on the client side with `localStorage`.  
- The application only needs to run locally, not in production.  
- All logs must use the **custom logging middleware**, not `console.log`.  

---

## 🛠 Error Handling

- Invalid URLs  
- Expired links  
- Duplicate shortcodes  
- Client-side input validation for URL format, shortcode format, and expiry time.  

---

## 📸 Screenshots

> Add screenshots here (Shortener Page, Stats Page, Redirect).  

---

## ✨ Future Enhancements

- 🔐 Add user authentication & authorization.  
- ☁️ Replace `localStorage` with a backend + database (MongoDB / PostgreSQL).  
- 📊 Enhanced analytics with charts & insights.  
- 🌍 Deploy to cloud (Vercel / Netlify).  

---

## 👨‍💻 Author

**Abhishek Srivastava**  
📧 [abhisheksriv6387@gmail.com](mailto:abhisheksriv6387@gmail.com)  
🔗 [LinkedIn](https://linkedin.com/in/your-link) |
