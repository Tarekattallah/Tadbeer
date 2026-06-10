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
[![Vite](https://img.shields.io/badge/Vite-5-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev)
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
| Agent Assignment | Admin assigns leads to sales agents |
| Activity Logging | Log calls, meetings, emails with timestamps per lead |
| Task Management | Create tasks with due dates, priorities, and reminders |
| Conversion Reports | Win/loss rate per agent, exportable to CSV |

### 👥 HRM Module — *Manage Your People. Automate the Rest.*

| Feature | Description |
|---------|-------------|
| Employee Directory | Full employee profiles with roles, departments, and contracts |
| Attendance Tracking | GPS-verified check-in/check-out with Late/Absent auto-detection |
| GPS Geofencing | Check-in only allowed within 100m of company location — location & distance recorded |
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
| 👤 | **Mahmoud** | Employee | Personal portal — check-in (GPS-verified), leave requests, own payslip |

> **Why no Super Admin?** Tadbeer serves a single organization. The Admin role (Sarah) holds full system control. A super-admin layer would add unnecessary complexity without business value.

---

## 🖥️ System Screens

### ✅ Completed (UI Design)

| # | Screen | Role(s) | Key Features |
|---|--------|---------|--------------|
| 1 | **Login Page** | All | Email/password auth, role-based redirect |
| 2 | **Admin Dashboard** | Admin | KPIs, revenue chart, recent activity feed |
| 3 | **CRM Client Hub** | Admin, Sales Agent | Lead stats, contacts table, lead detail panel |
| 4 | **HRM Employee Portal** | Admin, HR Manager | Attendance overview, team calendar, employee directory |
| 5 | **Leads List** | Admin, Sales Agent | Filterable lead table with status badges |

### 🔜 In Progress

| # | Screen | Priority | Purpose |
|---|--------|----------|---------|
| 6 | **Lead Details Page** | 🔴 HIGH | Full lead profile, activity timeline, embedded tasks |
| 7 | **Attendance Page** | 🔴 HIGH | GPS check-in/out, daily records, distance from office |
| 8 | **Leave Requests Page** | 🔴 HIGH | Pending/approved requests, approval workflow |
| 9 | **Payroll Page** | 🔴 HIGH | Monthly payroll table, generate payroll, payslips |
| 10 | **Employee Profile** | 🟡 MEDIUM | Individual data, contract, leave balance |
| 11 | **Sales Agent Dashboard** | 🟡 MEDIUM | Personal pipeline, tasks, activity summary |
| 12 | **Employee Self-Service** | 🟡 MEDIUM | GPS check-in, leave form, payslip download |
| 13 | **Settings Page** | 🟢 LOW | Company profile, user management |
| 14 | **Reports & Analytics** | 🟢 LOW | Conversion rates, HR stats, CSV export |

---

## 🛠️ Tech Stack

```
┌─────────────────────────────────────────────────┐
│              User Browser                        │
└────────────────────┬────────────────────────────┘
                     │
┌────────────────────▼────────────────────────────┐
│     Frontend: React 18 + Vite + Bootstrap 5      │
│     React Router · Axios · Leaflet (GPS map)     │
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
│        6 core collections · Embedded docs        │
└─────────────────────────────────────────────────┘
```

| Layer | Technology | Version | Purpose |
|-------|-----------|---------|---------|
| Runtime | Node.js | 20.x | Server runtime |
| Framework | Express.js | 4.x | REST API routing & middleware |
| ODM | Mongoose | 8.x | MongoDB schema & queries |
| Database | MongoDB | 7.x | NoSQL document storage |
| Frontend | React.js | 18.x | UI components & SPA routing |
| Bundler | Vite | 5.x | Fast dev server & build tool |
| Styling | Bootstrap | 5.x | Responsive UI components |
| Maps | Leaflet | — | GPS map display for attendance |
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
    ├──── leads (agentId ref → Employee)              │
    │       └── activities[]  ← embedded array        │
    │       └── tasks[]       ← embedded array        │
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
<summary><b>Lead Schema — with embedded Activities & Tasks</b> (click to expand)</summary>

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
  agentId:   { type: mongoose.Schema.Types.ObjectId, ref: 'Employee' },
  createdBy: { type: mongoose.Schema.Types.ObjectId, ref: 'Employee' },
  notes:     { type: String },

  // Embedded — no separate collections needed
  activities: [{
    type:      { type: String, enum: ['call', 'meeting', 'email', 'note'] },
    notes:     { type: String },
    createdBy: { type: mongoose.Schema.Types.ObjectId, ref: 'Employee' },
    createdAt: { type: Date, default: Date.now }
  }],

  tasks: [{
    title:      { type: String, required: true },
    dueDate:    { type: Date },
    priority:   { type: String, enum: ['high', 'medium', 'low'], default: 'medium' },
    status:     { type: String, enum: ['pending', 'done'], default: 'pending' },
    assignedTo: { type: mongoose.Schema.Types.ObjectId, ref: 'Employee' }
  }]
}, { timestamps: true });
```

> **Design decision:** Activities and Tasks are embedded inside Lead documents.
> This simplifies queries for the Lead Details page and avoids unnecessary joins.
> A Sales Agent will always access tasks/activities in the context of a specific lead.

</details>

<details>
<summary><b>Attendance Schema — with GPS Geofencing</b> (click to expand)</summary>

```js
const attendanceSchema = new mongoose.Schema({
  employeeId:   { type: mongoose.Schema.Types.ObjectId, ref: 'Employee', required: true },
  date:         { type: Date, required: true },
  checkIn:      { type: Date },
  checkOut:     { type: Date },
  locationIn: {
    lat: { type: Number },
    lng: { type: Number }
  },
  distanceIn:   { type: Number },   // metres from company location at check-in
  status:       { type: String, enum: ['Present', 'Late', 'Absent'], default: 'Present' },
  workingHours: { type: Number },
}, { timestamps: true });
```

> **GPS Geofencing:** Check-in is only enabled when the employee is within 100m of the
> company's registered location (calculated using the Haversine formula on the frontend).
> The location and distance are stored with every check-in record.
> HR Managers can view each employee's distance from the office in the attendance table.

</details>

<details>
<summary><b>LeaveRequest Schema</b> (click to expand)</summary>

```js
const leaveRequestSchema = new mongoose.Schema({
  employeeId: { type: mongoose.Schema.Types.ObjectId, ref: 'Employee', required: true },
  type:       { type: String, enum: ['annual', 'sick', 'emergency'], required: true },
  startDate:  { type: Date, required: true },
  endDate:    { type: Date, required: true },
  reason:     { type: String },
  status:     { type: String, enum: ['Pending', 'Approved', 'Rejected'], default: 'Pending' },
  reviewedBy: { type: mongoose.Schema.Types.ObjectId, ref: 'Employee' },
  reviewNote: { type: String },
}, { timestamps: true });
```

</details>

<details>
<summary><b>Payroll Schema</b> (click to expand)</summary>

```js
const payrollSchema = new mongoose.Schema({
  employeeId:  { type: mongoose.Schema.Types.ObjectId, ref: 'Employee', required: true },
  month:       { type: String, required: true },   // "2025-06"
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
GET    /api/leads/:id              → Lead details + embedded activities + tasks
PUT    /api/leads/:id              → Update lead
DELETE /api/leads/:id              → Delete lead                    [admin]
PATCH  /api/leads/:id/assign       → Assign to agent                [admin]
PATCH  /api/leads/:id/status       → Update pipeline status
```

### CRM — Activities & Tasks (embedded in Lead)
```
POST   /api/leads/:id/activities        → Log activity (call/meeting/email/note)
DELETE /api/leads/:id/activities/:actId → Remove activity            [admin]

POST   /api/leads/:id/tasks             → Add task to lead
PATCH  /api/leads/:id/tasks/:taskId     → Update task (status, priority)
DELETE /api/leads/:id/tasks/:taskId     → Remove task
```

### HRM — Employees
```
GET    /api/employees              → List all employees    [admin, hr_manager]
POST   /api/employees              → Create employee       [admin, hr_manager]
GET    /api/employees/:id          → Get employee details  [admin, hr_manager]
PUT    /api/employees/:id          → Update employee       [admin, hr_manager]
DELETE /api/employees/:id          → Deactivate employee   [admin]
```

### HRM — Attendance (GPS-enabled)
```
POST   /api/attendance/checkin         → Record check-in (lat, lng required)  [employee]
POST   /api/attendance/checkout        → Record check-out                      [employee]
GET    /api/attendance                 → All records with distance column       [admin, hr_manager]
GET    /api/attendance/my              → Own records                            [employee]
GET    /api/attendance/:employeeId     → Specific employee records              [admin, hr_manager]
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
GET    /api/payroll/my                 → Own payslips               [all roles]
GET    /api/payroll/:id/pdf            → Download payslip PDF       [admin, hr_manager, self]
```

### Notifications
```
GET    /api/notifications              → Current user notifications
PATCH  /api/notifications/read         → Mark all as read
```

> **Validation:** All request bodies are validated using **Joi**. Invalid requests return `400`. Auth errors return `401`. Permission errors return `403`.

---

## 🔐 Permissions Matrix

| Feature | Admin | Sales Agent | HR Manager | Employee |
|---------|:-----:|:-----------:|:----------:|:--------:|
| View All Leads | ✅ | Own only | ❌ | ❌ |
| Add New Lead | ✅ | ✅ | ❌ | ❌ |
| Assign Lead to Agent | ✅ | ❌ | ❌ | ❌ |
| Log Activities & Tasks | ✅ | Own leads only | ❌ | ❌ |
| View CRM Reports | ✅ | ❌ | ❌ | ❌ |
| Manage Employees | ✅ | ❌ | ✅ | ❌ |
| View All Attendance | ✅ | ❌ | ✅ | ❌ |
| GPS Check In / Check Out | ❌ | ❌ | ❌ | ✅ |
| Approve Leave Requests | ✅ | ❌ | ✅ | ❌ |
| Submit Leave Request | ✅ | ✅ | ✅ | ✅ |
| Generate Monthly Payroll | ✅ | ❌ | ✅ | ❌ |
| View Own Payslip | ✅ | ✅ | ✅ | ✅ |
| System Settings | ✅ | ❌ | ❌ | ❌ |

---

## 📋 User Stories

<details>
<summary><b>🎯 Scenario 1 — Layla adds a lead and closes the deal</b></summary>

Layla logs into her Sales Agent portal. She adds **Pizza House** as a new lead with contact details and expected value. She adds a task "Demo call — Thursday 2PM". After the call, she logs it as an Activity with outcome notes. The lead moves through `Contacted → Negotiation` and she marks it **Won**. Sarah sees the revenue chart update on her Admin Dashboard.

</details>

<details>
<summary><b>👥 Scenario 2 — Karim approves a leave request</b></summary>

Karim opens the HRM portal and sees a **Pending** leave request from Mahmoud for 3 annual days. He reviews the dates and clicks **Approve**. The system auto-deducts 3 days from Mahmoud's 21-day balance and sends him a notification.

</details>

<details>
<summary><b>💰 Scenario 3 — Karim generates monthly payroll</b></summary>

At month end, Karim clicks **Generate Payroll**. The system calculates each employee's net salary: `Basic Salary + Bonuses − Deductions`. PDF payslips are generated and pushed to each employee's personal portal.

</details>

<details>
<summary><b>🗺️ Scenario 4 — Mahmoud records GPS attendance</b></summary>

Mahmoud arrives at 9:05 AM and opens his Employee portal. The system checks his GPS location — he is 15m from the office, within the 100m allowed radius. The Check-in button is enabled. He taps it — the system records his arrival time, location, and flags him **Late (5 min)**. At end of day he taps Check Out. HR Manager Karim can see Mahmoud's distance from the office in the attendance table.

</details>

<details>
<summary><b>📊 Scenario 5 — Sarah monitors sales performance</b></summary>

Sarah opens the Admin Dashboard and navigates to **CRM Reports**. She sees Won vs Lost deals per agent for the current quarter, overall conversion rates, and monthly trends. She exports the data to **CSV** for the board meeting.

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
│   │   ├── Employee.js               # includes role, salary, leaveBalance
│   │   ├── Lead.js                   # includes embedded activities[] & tasks[]
│   │   ├── Attendance.js             # includes GPS locationIn & distanceIn
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
│   │   ├── lead.controller.js        # handles embedded activities & tasks too
│   │   ├── employee.controller.js
│   │   ├── attendance.controller.js  # handles GPS validation logic
│   │   ├── leave.controller.js
│   │   └── payroll.controller.js
│   ├── validators/                   # Joi schemas per resource
│   │   ├── auth.validator.js
│   │   ├── lead.validator.js
│   │   ├── employee.validator.js
│   │   └── leave.validator.js
│   ├── utils/
│   │   ├── generatePayslip.js        # PDFKit — build payslip PDF
│   │   └── sendNotification.js       # Create in-app notification document
│   ├── seed/
│   │   └── seed.js                   # Seeds 4 demo users, 10 leads, attendance records
│   ├── .env.example
│   ├── package.json
│   └── server.js                     # Entry point
│
└── frontend/                         # React 18 + Vite + Bootstrap 5
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
git clone https://github.com/Tarekattallah/tadbeer.git
cd tadbeer/backend

# 2. Install dependencies
npm install

# 3. Configure environment
cp .env.example .env
# Edit .env with your values (see Environment Variables section)

# 4. Seed demo data
node seed/seed.js
# Creates: 4 demo users (one per role), 10 sample leads, attendance records

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
# Local:  mongodb://localhost:27017/tadbeer
# Atlas:  mongodb+srv://user:pass@cluster.mongodb.net/tadbeer

# ── Authentication ────────────────────────
JWT_SECRET=your_super_secret_key_change_this_in_production
JWT_EXPIRES_IN=7d

# ── Company Location (for GPS Geofencing) ─
COMPANY_LAT=30.0525
COMPANY_LNG=31.2387
COMPANY_RADIUS=100

# ── File Storage ──────────────────────────
UPLOAD_PATH=./uploads
MAX_FILE_SIZE=5mb
```

> ⚠️ Never commit your real `.env` file. Make sure it's listed in `.gitignore`.

---

## 🗺️ Roadmap

| Sprint | Duration | Deliverables | Status |
|--------|----------|-------------|--------|
| 1 | Week 1 | Project setup, Mongoose models, JWT auth (login + protect + RBAC) | ⏳ Pending |
| 2 | Week 2 | Leads CRUD + embedded activities & tasks APIs + Joi validation | ⏳ Pending |
| 3 | Week 3 | Employees CRUD + Attendance (GPS check-in/out) + Leave APIs | ⏳ Pending |
| 4 | Week 4 | Payroll generation + PDF payslips + Notifications | ⏳ Pending |
| 5 | Week 5 | React app — Login, Sidebar, Admin Dashboard, Leads List | ⏳ Pending |
| 6 | Week 6 | Lead Details page (timeline + tasks) + GPS Attendance page (Leaflet map) | ⏳ Pending |
| 7 | Week 7 | HRM pages — Employees, Leave Requests, Payroll + Employee self-service | ⏳ Pending |
| 8 | Week 8 | Dashboards (Admin, Agent, HR, Employee) + Reports + CSV export | ⏳ Pending |
| 9 | Week 9 | Testing, bug fixes, seed data polish, presentation prep | ⏳ Pending |

---

## 📄 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

**Tadbeer — تدبير**

*Graduation Project · TechNile CRM + HRM Platform · 2025*

Built with ❤️ using Node.js + Express + MongoDB + React + Vite + Bootstrap

</div>
