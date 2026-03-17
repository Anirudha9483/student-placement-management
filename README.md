# 🎨 Frontend Development Plan (React.js + Bootstrap)

This document outlines the **frontend development structure** for the *Student Interview & Resume Tracking System*, divided among **3 team members** to ensure efficient and parallel development.

---

## 🚀 Frontend Tech Stack

* React.js
* Bootstrap 5
* React Router DOM
* Axios

---

## 👥 Team Division (Frontend Only)

---

## 👨‍💻 Member 1: UI / Layout Developer

### 🎯 Responsibility:

Design and build the **visual structure** of the application using Bootstrap.

### 📌 Tasks:

* Create reusable UI components:

  * Navbar
  * Sidebar
  * Footer
* Design layout structure:

  * Dashboard layout
  * Page containers
* Apply Bootstrap styling:

  * Grid system
  * Cards
  * Buttons
* Ensure responsive design (mobile + desktop)

### 📂 Components to Build:

```id="m1comp"
components/
├── Navbar.jsx
├── Sidebar.jsx
├── Footer.jsx
├── Layout.jsx
```

---

## 👨‍💻 Member 2: Student & Form Management

### 🎯 Responsibility:

Handle all **form-based features** and student-related UI + logic.

### 📌 Tasks:

* Build Student Form:

  * Add / Edit student
* Create Student List:

  * Display data in table
* Add validation:

  * Required fields
  * Email format
* Handle basic state (useState)

### 📂 Components to Build:

```id="m2comp"
components/
├── StudentForm.jsx
├── StudentList.jsx
├── StudentCard.jsx
```

---

## 👨‍💻 Member 3: Dashboard & API Integration

### 🎯 Responsibility:

Handle **data flow, API integration, and dashboard logic**

### 📌 Tasks:

* Create Dashboard:

  * Total students
  * Resume uploaded
  * Mock interview stats
* Setup Axios API calls
* Manage global state (basic)
* Integrate backend APIs
* Handle routing

### 📂 Components to Build:

```id="m3comp"
components/
├── Dashboard.jsx
├── StatsCard.jsx

services/
├── api.js
```

---

## 📁 Page Structure

```id="pagestruct"
pages/
├── Home.jsx
├── Students.jsx
├── DashboardPage.jsx
```

---

## 🔀 Routing Setup

```jsx id="routingcode"
import { BrowserRouter as Router, Routes, Route } from "react-router-dom";
import DashboardPage from "./pages/DashboardPage";
import Students from "./pages/Students";

function App() {
  return (
    <Router>
      <Routes>
        <Route path="/" element={<DashboardPage />} />
        <Route path="/students" element={<Students />} />
      </Routes>
    </Router>
  );
}

export default App;
```

---

## 🤝 Collaboration Strategy

### 🔄 Workflow:

* Member 1 builds UI structure first
* Member 2 integrates forms into UI
* Member 3 connects APIs and dashboard data

### 🔗 Integration Order:

1. Layout (Navbar + Sidebar)
2. Pages setup
3. Student module
4. Dashboard
5. API integration

---

## 📅 Suggested Timeline

| Day     | Task                   |
| ------- | ---------------------- |
| Day 1–2 | Project setup + Layout |
| Day 3–4 | Student module UI      |
| Day 5–6 | Dashboard UI           |
| Day 7   | API integration        |
| Day 8   | Testing & fixes        |

---

## ✅ Best Practices

* Use reusable components
* Keep code modular
* Use consistent naming conventions
* Separate UI and logic
* Test components individually

---

## 📌 Final Goal

✔ Clean UI using Bootstrap
✔ Fully functional frontend
✔ Connected to backend APIs
✔ Responsive design

---

### ⭐ Teamwork Tip:

Communicate daily and push code regularly to GitHub for smooth collaboration.
