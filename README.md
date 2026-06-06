<div align="center">

<img src="https://img.shields.io/badge/Tadbeer-تدبير-00D4C8?style=for-the-badge&labelColor=0D1B2A&color=00D4C8" height="40"/>

# Tadbeer — تدبير

### Integrated CRM + HRM Web Platform

**Built for TechNile · RestoSoft Sales Operations · Graduation Project 2025**

---

[![Node.js](https://img.shields.io/badge/Node.js-20-339933?style=flat-square&logo=nodedotjs&logoColor=white)](https://nodejs.org)
[![Express](https://img.shields.io/badge/Express-4-000000?style=flat-square&logo=express&logoColor=white)](https://expressjs.com)
[![MongoDB](https://img.shields.io/badge/MongoDB-7-47A248?style=flat-square&logo=mongodb&logoColor=white)](https://mongodb.com)
[![Mongoose](https://img.shields.io/badge/Mongoose-ODM-880000?style=flat-square&logo=mongoose&logoColor=white)](https://mongoosejs.com)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black)](https://react.dev)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5-7952B3?style=flat-square&logo=bootstrap&logoColor=white)](https://getbootstrap.com)
[![JWT](https://img.shields.io/badge/Auth-JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)](https://jwt.io)
[![Joi](https://img.shields.io/badge/Validation-Joi-0080FF?style=flat-square)](https://joi.dev)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![Status](https://img.shields.io/badge/Status-In%20Development-orange?style=flat-square)]()

</div>

---

## 📖 Table of Contents

- [Overview](#-overview)
- [The Problem](#-the-problem)
- [Modules](#-modules)
- [User Roles](#-user-roles)
- [System Screens](#-system-screens)
- [Tech Stack](#-tech-stack)
- [Database Schema](#-database-schema)
- [API Reference](#-api-reference)
- [Permissions Matrix](#-permissions-matrix)
- [User Stories](#-user-stories)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [Roadmap](#-roadmap)

---

## 🌐 Overview

**Tadbeer (تدبير)** is a full-stack, role-based web platform that unifies two critical business operations — **CRM** and **HRM** — into a single, centralized system built for **TechNile**, a fictional Egyptian software company that sells *RestoSoft* to restaurants.

> **"One system. Every role. Total control."**

The platform replaces fragmented Excel files and paper-based workflows with a modern, secure, and permission-aware web application that gives every team member exactly what they need — nothing more, nothing less.

---

## 🔴 The Problem

Before Tadbeer, TechNile faced three core operational failures:

| Problem | Impact |
|--------|--------|
| ❌ **No lead tracking** | Sales agents forgot to follow up with restaurant clients. Deals were lost with no record. |
| ❌ **Paper-based HR** | Attendance on WhatsApp. Leave requests by phone. Payroll calculated manually in Excel. |
| ❌ **Zero visibility** | Management had no real-time view of sales performance, employee status, or company metrics. |

**Tadbeer solves all three.**

---

## 📦 Modules

### 🎯 CRM Module — *Track Every Lead. Close Every Deal.*

| Feature | Description |
|---------|-------------|
| Lead Pipeline | Full lifecycle: `New → Assigned → Contacted → Negotiation → Won / Lost` |
| Agent Assignment | Admin assigns leads to sales agents automatically |
| Activity Logging | Log calls, meetings, emails with timestamps per lead |
| Task Management | Create tasks with due dates, priorities, and reminders |
| Conversion Reports | Win/loss rate per agent, exportable to CSV |

### 👥 HRM Module — *Manage Your People. Automate the Rest.*

| Feature | Description |
|---------|-------------|
| Employee Directory | Full employee profiles with roles, departments, and contracts |
| Attendance Tracking | Daily check-in/check-out with Late/Absent auto-detection |
| Leave Requests | Submit, approve, or reject — balance auto-deducted on approval |
| Payroll Automation | Monthly net salary: `Base + Bonuses − Deductions` |
| Payslip PDF | Auto-generated payslips downloadable from employee portal |

---

## 👤 User Roles

Tadbeer is built around **4 core roles**. The highest authority is **Admin** — no super-admin exists because the system is designed for a single company (TechNile).

| Avatar | Name | Role | Access Level |
|--------|------|------|-------------|
| 📊 | **Sarah** | Admin / General Manager | Highest authority — full CRM + HRM overview, reports, payroll approval, user management |
| 🧑‍💼 | **Karim** | HR Manager | HRM only — employees, attendance, leave requests, payroll generation |
| 🎯 | **Layla** | Sales Agent | Her own leads, tasks, and activities only |
| 👤 | **Mahmoud** | Employee | Personal portal — check-in, leave requests, own payslip |

> **Why no Super Admin?** Tadbeer serves a single organization. The Admin role (Sarah) holds full system control. A super-admin layer would add unnecessary complexity without business value.

---

## 🖥️ System Screens

### ✅ Completed

| # | Screen | Role(s) | Key Features |
|---|--------|---------|--------------|
| 1 | **Login Page** | All | Email/password auth, role-based redirect |
| 2 | **Admin Dashboard** | Admin | KPIs, revenue chart, recent activity feed |
| 3 | **CRM Client Hub** | Admin, Sales Agent | Lead stats, contacts table, lead detail panel |
| 4 | **HRM Employee Portal** | Admin, HR Manager | Attendance overview, team calendar, employee directory |
| 5 | **Project Tracking** | Admin, Sales, Support | Budget, Kanban board (Backlog / In Progress / Review / Done) |
| 6 | **Leads List** | Admin, Sales Agent | Filterable lead table with status badges |

### 🔜 In Progress

| # | Screen | Priority | Purpose |
|---|--------|----------|---------|
| 7 | **Lead Details Page** | 🔴 HIGH | Full lead profile, activity timeline, tasks |
| 8 | **Attendance Page** | 🔴 HIGH | Daily records, filter by employee/date |
| 9 | **Leave Requests Page** | 🔴 HIGH | Pending/approved requests, approval workflow |
| 10 | **Payroll Page** | 🔴 HIGH | Monthly payroll table, generate payroll, payslips |
| 11 | **Employee Profile** | 🟡 MEDIUM | Individual data, contract, leave balance |
| 12 | **Sales Agent Dashboard** | 🟡 MEDIUM | Personal pipeline, tasks, activity summary |
| 13 | **Employee Self-Service** | 🟡 MEDIUM | Check-in, leave form, payslip download |
| 14 | **Settings Page** | 🟢 LOW | Company profile, user management |
| 15 | **Reports & Analytics** | 🟢 LOW | Conversion rates, HR stats, CSV export |

---

## 🛠️ Tech Stack

```
┌─────────────────────────────────────────────────┐
│              User Browser                        │
└────────────────────┬────────────────────────────┘
                     │
┌────────────────────▼────────────────────────────┐
│       Frontend: React 18 + Bootstrap 5           │
│       React Router · Axios · React Bootstrap     │
└────────────────────┬────────────────────────────┘
                     │  REST API (HTTP/HTTPS + JSON)
┌────────────────────▼────────────────────────────┐
│         Backend: Node.js + Express 4             │
│   JWT Auth · RBAC Middleware · Joi Validation    │
│   Mongoose ODM · Multer · PDFKit                 │
└────────────────────┬────────────────────────────┘
                     │
┌────────────────────▼────────────────────────────┐
│            Database: MongoDB (Mongoose)          │
│     6 core collections · GridFS file storage    │
└─────────────────────────────────────────────────┘
```

| Layer | Technology | Version | Purpose |
|-------|-----------|---------|---------|
| Runtime | Node.js | 20.x | Server runtime |
| Framework | Express.js | 4.x | REST API routing & middleware |
| ODM | Mongoose | 8.x | MongoDB schema & queries |
| Database | MongoDB | 7.x | NoSQL document storage |
| Frontend | React.js | 18.x | UI components & SPA routing |
| Styling | Bootstrap | 5.x | Responsive UI components |
| Auth | JSON Web Tokens (JWT) | — | Stateless session management |
| Validation | Joi | — | Request body validation |
| PDF | PDFKit | — | Monthly payslip generation |
| File Upload | Multer | — | Employee docs & attachments |

---

## 🗄️ Database Schema (MongoDB Collections)

```
employees ───────────────────────────────────────────┐
    │  role: ['admin','sales_agent','hr_manager',     │
    │          'employee']                            │
    │  department: ['management','sales','hr',        │
    │               'support']                        │
    │                                                 │
    ├──── leads        (agentId ref → Employee)       │
    │       └── activities  (leadId ref → Lead)       │
    │       └── tasks        (leadId ref → Lead)      │
    │                                                 │
    ├──── attendance    (employeeId ref → Employee)   │
    ├──── leaveRequests (employeeId ref → Employee)   │
    ├──── payroll       (employeeId ref → Employee)   │
    └──── notifications (userId    ref → Employee)  ◄─┘
```

### Mongoose Schemas

<details>
<summary><b>Employee Schema</b> (click to expand)</summary>

```js
const employeeSchema = new mongoose.Schema({
  name:         { type: String, required: true },
  email:        { type: String, required: true, unique: true },
  password:     { type: String, required: true },  // bcrypt hashed
  phone:        { type: String },
  role: {
    type: String,
    enum: ['admin', 'sales_agent', 'hr_manager', 'employee'],
    required: true
  },
  department: {
    type: String,
    enum: ['management', 'sales', 'hr', 'support']
  },
  basicSalary:  { type: Number, default: 0 },
  leaveBalance: { type: Number, default: 21 },
  hireDate:     { type: Date },
  isActive:     { type: Boolean, default: true },
}, { timestamps: true });
```

</details>

<details>
<summary><b>Lead Schema</b> (click to expand)</summary>

```js
const leadSchema = new mongoose.Schema({
  restaurantName: { type: String, required: true },
  contactPerson:  { type: String },
  phone:          { type: String },
  email:          { type: String },
  expectedValue:  { type: Number, default: 0 },
  status: {
    type: String,
    enum: ['New', 'Assigned', 'Contacted', 'Negotiation', 'Won', 'Lost'],
    default: 'New'
  },
  agentId:    { type: mongoose.Schema.Types.ObjectId, ref: 'Employee' },
  createdBy:  { type: mongoose.Schema.Types.ObjectId, ref: 'Employee' },
  notes:      { type: String },
}, { timestamps: true });
```

</details>

<details>
<summary><b>Attendance Schema</b> (click to expand)</summary>

```js
const attendanceSchema = new mongoose.Schema({
  employeeId:   { type: mongoose.Schema.Types.ObjectId, ref: 'Employee', required: true },
  date:         { type: Date, required: true },
  checkIn:      { type: String },       // "09:05"
  checkOut:     { type: String },       // "17:30"
  status:       { type: String, enum: ['Present', 'Late', 'Absent'], default: 'Present' },
  workingHours: { type: Number },
}, { timestamps: true });
```

</details>

<details>
<summary><b>Payroll Schema</b> (click to expand)</summary>

```js
const payrollSchema = new mongoose.Schema({
  employeeId:  { type: mongoose.Schema.Types.ObjectId, ref: 'Employee', required: true },
  month:       { type: String, required: true },   // "2025-01"
  basicSalary: { type: Number },
  bonuses:     { type: Number, default: 0 },
  deductions:  { type: Number, default: 0 },
  netSalary:   { type: Number },    // basicSalary + bonuses - deductions
  status:      { type: String, enum: ['Pending', 'Paid'], default: 'Pending' },
  payslipUrl:  { type: String },    // PDF download path
}, { timestamps: true });
```

</details>

---

## 🔌 API Reference

**Base URL:** `http://localhost:5000/api`

> All protected routes require the header:
> `Authorization: Bearer <token>`
>
> Every endpoint uses two middleware layers:
> - `protect` — verifies JWT and attaches `req.user`
> - `authorize('admin', 'hr_manager')` — checks role permission

### Authentication
```
POST   /api/auth/login       → Login → returns JWT token
POST   /api/auth/logout      → Logout (blacklist token)
GET    /api/auth/me          → Get current user profile
```

### CRM — Leads
```
GET    /api/leads                  → List leads (auto-filtered by role)
POST   /api/leads                  → Create new lead
GET    /api/leads/:id              → Lead details + activities + tasks
PUT    /api/leads/:id              → Update lead
DELETE /api/leads/:id              → Delete lead           [admin]
PATCH  /api/leads/:id/assign       → Assign to agent       [admin]
PATCH  /api/leads/:id/status       → Update pipeline status
```

### CRM — Activities & Tasks
```
POST   /api/leads/:id/activities   → Log activity (call/meeting/email/note)
GET    /api/leads/:id/activities   → Get activity timeline
POST   /api/leads/:id/tasks        → Add task to lead
GET    /api/tasks                  → List tasks (filtered by role)
PATCH  /api/tasks/:id/status       → Mark task done / pending
```

### HRM — Employees
```
GET    /api/employees              → List all employees    [admin, hr_manager]
POST   /api/employees              → Create employee       [admin, hr_manager]
GET    /api/employees/:id          → Get employee details  [admin, hr_manager]
PUT    /api/employees/:id          → Update employee       [admin, hr_manager]
DELETE /api/employees/:id          → Deactivate employee   [admin]
```

### HRM — Attendance
```
POST   /api/attendance/checkin         → Record check-in      [employee]
POST   /api/attendance/checkout        → Record check-out     [employee]
GET    /api/attendance                 → All records          [admin, hr_manager]
GET    /api/attendance/my              → Own records          [employee]
GET    /api/attendance/:employeeId     → Specific employee    [admin, hr_manager]
```

### HRM — Leave Requests
```
GET    /api/leaves                     → All requests         [admin, hr_manager]
GET    /api/leaves/my                  → Own requests         [all roles]
POST   /api/leaves                     → Submit leave request [all roles]
PATCH  /api/leaves/:id/approve         → Approve              [admin, hr_manager]
PATCH  /api/leaves/:id/reject          → Reject with comment  [admin, hr_manager]
```

### HRM — Payroll
```
POST   /api/payroll/generate           → Generate monthly payroll  [admin, hr_manager]
GET    /api/payroll                    → View payroll list          [admin, hr_manager]
GET    /api/payroll/my                 → Own payslip               [all roles]
GET    /api/payroll/:id/pdf            → Download payslip PDF      [admin, hr_manager, self]
```

### Notifications
```
GET    /api/notifications              → Current user notifications
PATCH  /api/notifications/read         → Mark all as read
```

> **Validation:** All request bodies are validated using **Joi**. Invalid requests return `400` with a descriptive error message. Auth errors return `401`. Permission errors return `403`.

---

## 🔐 Permissions Matrix

| Feature | Admin | Sales Agent | HR Manager | Employee |
|---------|:-----:|:-----------:|:----------:|:--------:|
| View All Leads | ✅ | Own only | ❌ | ❌ |
| Add New Lead | ✅ | ✅ | ❌ | ❌ |
| Assign Lead to Agent | ✅ | ❌ | ❌ | ❌ |
| Log Activities & Tasks | ✅ | Own only | ❌ | ❌ |
| View CRM Reports | ✅ | ❌ | ❌ | ❌ |
| Manage Employees | ✅ | ❌ | ✅ | ❌ |
| View All Attendance | ✅ | ❌ | ✅ | ❌ |
| Check In / Check Out | ❌ | ❌ | ❌ | ✅ |
| Approve Leave Requests | ✅ | ❌ | ✅ | ❌ |
| Submit Leave Request | ✅ | ✅ | ✅ | ✅ |
| Generate Monthly Payroll | ✅ | ❌ | ✅ | ❌ |
| View Own Payslip | ✅ | ✅ | ✅ | ✅ |
| System Settings | ✅ | ❌ | ❌ | ❌ |

---

## 📋 User Stories

<details>
<summary><b>🎯 Scenario 1 — Layla adds a lead and closes the deal</b></summary>

Layla logs into her Sales Agent portal. She adds **Pizza House** as a new lead, fills in the contact details and expected value. She schedules a call task for **Thursday 2PM**. After the call, she logs it as an Activity with outcome notes. The lead moves through `Contacted → Negotiation` and finally she marks it as **Won**. Sarah receives an instant notification and sees the revenue chart update on her dashboard.

</details>

<details>
<summary><b>👥 Scenario 2 — Karim approves a leave request</b></summary>

Karim opens the HRM portal and sees a **Pending** leave request from Mahmoud for 3 annual days. He reviews the dates and clicks **Approve**. The system auto-deducts 3 days from Mahmoud's 21-day balance, sends him a notification, and marks those days on the team attendance calendar.

</details>

<details>
<summary><b>💰 Scenario 3 — Karim generates monthly payroll</b></summary>

At the end of the month, Karim clicks **Generate Payroll**. The system calculates each employee's net salary: `Basic Salary + Bonuses − Deductions`. Individual PDF payslips are generated and pushed to each employee's personal portal for download.

</details>

<details>
<summary><b>🕘 Scenario 4 — Mahmoud records daily attendance</b></summary>

Mahmoud arrives at 9:05 AM and opens his Employee portal. He taps **Check In** — the system records his arrival and flags him as **Late (5 minutes)**. At end of day he taps **Check Out**. He can view his full monthly attendance history with working hours per day.

</details>

<details>
<summary><b>📊 Scenario 5 — Sarah monitors sales performance</b></summary>

Sarah opens the Admin Dashboard and navigates to **CRM Reports**. She sees a breakdown of Won vs Lost deals per agent for the current quarter, overall conversion rates, and monthly trends. She exports the data to **CSV** for the board meeting.

</details>

---

## 📁 Project Structure

```
tadbeer/
│
├── backend/                          # Node.js + Express API
│   ├── config/
│   │   └── db.js                     # MongoDB connection via Mongoose
│   ├── middleware/
│   │   ├── auth.js                   # protect() — verify JWT, attach req.user
│   │   ├── rbac.js                   # authorize(...roles) — check role permission
│   │   └── validate.js               # Joi validation wrapper
│   ├── models/
│   │   ├── Employee.js
│   │   ├── Lead.js
│   │   ├── Activity.js
│   │   ├── Task.js
│   │   ├── Attendance.js
│   │   ├── LeaveRequest.js
│   │   ├── Payroll.js
│   │   └── Notification.js
│   ├── routes/
│   │   ├── auth.routes.js
│   │   ├── lead.routes.js
│   │   ├── employee.routes.js
│   │   ├── attendance.routes.js
│   │   ├── leave.routes.js
│   │   ├── payroll.routes.js
│   │   └── notification.routes.js
│   ├── controllers/
│   │   ├── auth.controller.js
│   │   ├── lead.controller.js
│   │   ├── employee.controller.js
│   │   ├── attendance.controller.js
│   │   ├── leave.controller.js
│   │   └── payroll.controller.js
│   ├── validators/                   # Joi schemas per resource
│   │   ├── lead.validator.js
│   │   ├── employee.validator.js
│   │   └── leave.validator.js
│   ├── utils/
│   │   ├── generatePayslip.js        # PDFKit — build payslip PDF
│   │   └── sendNotification.js       # Create in-app notification
│   ├── seed/
│   │   └── seed.js                   # Seeds 4 roles, 4 demo users,
│   │                                 # 10 leads, sample attendance
│   ├── .env.example
│   ├── package.json
│   └── server.js                     # Entry point
│
└── frontend/                         # React 18 + Bootstrap 5
    ├── public/
    └── src/
        ├── pages/
        │   ├── auth/           Login.jsx
        │   ├── admin/          Dashboard.jsx · Settings.jsx
        │   ├── crm/            LeadsList.jsx · LeadDetails.jsx · NewLead.jsx
        │   └── hrm/            Employees.jsx · Attendance.jsx
        │                       LeaveRequests.jsx · Payroll.jsx
        ├── components/
        │   ├── layout/         Sidebar.jsx · Navbar.jsx · Footer.jsx
        │   └── ui/             StatusBadge.jsx · RoleGuard.jsx · KpiCard.jsx
        ├── context/
        │   └── AuthContext.jsx         # JWT storage + current user state
        ├── hooks/
        │   └── useAuth.js
        ├── api/
        │   └── axios.js                # Axios instance + JWT interceptor
        ├── App.jsx
        └── main.jsx
```

---

## 🚀 Getting Started

### Prerequisites

- Node.js 20+
- MongoDB (local) or [MongoDB Atlas](https://www.mongodb.com/atlas) (cloud)
- npm or yarn

### Backend Setup

```bash
# 1. Clone the repo
git clone https://github.com/your-username/tadbeer.git
cd tadbeer/backend

# 2. Install dependencies
npm install

# 3. Configure environment
cp .env.example .env
# Edit .env with your values (see Environment Variables section)

# 4. Seed demo data
node seed/seed.js
# Creates: 4 roles, 4 demo users, 10 sample leads, attendance records

# 5. Start the server
npm run dev      # development — nodemon auto-restart
npm start        # production
```

### Frontend Setup

```bash
cd ../frontend

npm install

cp .env.example .env
# Set VITE_API_URL=http://localhost:5000/api

npm run dev
```

### Default Login Credentials (after seeding)

| Role | Email | Password |
|------|-------|----------|
| Admin | sarah@technile.com | password123 |
| HR Manager | karim@technile.com | password123 |
| Sales Agent | layla@technile.com | password123 |
| Employee | mahmoud@technile.com | password123 |

---

## ⚙️ Environment Variables

Copy `.env.example` to `.env` and fill in the values:

```env
# ── Server ────────────────────────────────
PORT=5000
NODE_ENV=development

# ── Database ──────────────────────────────
MONGO_URI=your_mongodb_connection_string
# Local example:  mongodb://localhost:27017/tadbeer
# Atlas example:  mongodb+srv://user:pass@cluster.mongodb.net/tadbeer

# ── Authentication ────────────────────────
JWT_SECRET=your_super_secret_key_change_this_in_production
JWT_EXPIRES_IN=7d

# ── Email (optional — for notifications) ──
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password

# ── File Storage ──────────────────────────
UPLOAD_PATH=./uploads
MAX_FILE_SIZE=5mb
```

> ⚠️ Never commit your real `.env` file. Make sure it's listed in `.gitignore`.

---

## 🗺️ Roadmap

| Phase | Duration | Deliverables | Status |
|-------|----------|-------------|--------|
| 1 | Week 1 | MongoDB setup, Mongoose models, JWT auth | ✅ Done |
| 2 | Week 2 | Leads & Employees CRUD APIs + Joi validation | ✅ Done |
| 3 | Week 3 | Attendance, Leave, Payroll APIs | 🔄 In Progress |
| 4 | Week 4 | React app — Login, Admin Dashboard, Sidebar | ✅ Done |
| 5 | Week 5 | CRM pages — Leads List, Lead Details | 🔄 In Progress |
| 6 | Week 6 | HRM pages — Employees, Attendance, Leave, Payroll | ⏳ Pending |
| 7 | Week 7 | Sales Agent & Employee self-service portals | ⏳ Pending |
| 8 | Week 8 | Reports, Notifications, Settings, PDF payslips | ⏳ Pending |
| 9 | Week 9 | Testing, bug fixes, documentation, presentation | ⏳ Pending |

---

## 📄 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

**Tadbeer — تدبير**

*Graduation Project · TechNile CRM + HRM Platform · 2025*

Built with ❤️ using Node.js + Express + MongoDB + React + Bootstrap

</div>
