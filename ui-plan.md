# LMS Project – UI Component Plan

## 🎯 Goal
Design a scalable and reusable frontend structure for the LMS (Learning Management System) project using **Next.js (App Router)** and **Tailwind CSS**.

---

## 🧩 Core Layout Components

| Component | Description | Reusability |
|------------|--------------|--------------|
| **Navbar** | Displays logo, navigation links (Home, Courses, Dashboard, Login/Logout) | Shared across all pages |
| **Footer** | Displays copyright info and site links | Shared across all pages |
| **DashboardLayout** | Wrapper layout for authenticated pages with sidebar navigation | Used in admin and student dashboards |
| **Sidebar** | Contains links for "Courses", "Progress", "Profile" | Used inside DashboardLayout |
| **Button** | Reusable button component with Tailwind variants (primary, secondary) | Used across forms and pages |
| **Input** | Reusable input component for forms | Used in Login, Signup, and Course creation forms |
| **CourseCard** | Displays course title, description, and "Enroll" button | Used on student dashboard and course listing page |

---

## 📄 Page-Level Components

| Page | Description |
|------|--------------|
| **Home Page (`app/page.js`)** | Landing page with welcome section and CTA buttons |
| **Login Page (`app/login/page.js`)** | Contains a login form using reusable Input and Button components |
| **Dashboard Page (`app/dashboard/page.js`)** | Displays student or admin dashboard layout |
| **Courses Page (`app/courses/page.js`)** | Lists all available courses using `CourseCard` components |

---

## 🗂️ Folder Structure

lms-project/
│
├── app/
│ ├── layout.js
│ ├── page.js
│ ├── login/
│ │ └── page.js
│ ├── dashboard/
│ │ └── page.js
│ ├── courses/
│ │ └── page.js
│
├── components/
│ ├── Navbar.js
│ ├── Footer.js
│ ├── DashboardLayout.js
│ ├── Sidebar.js
│ ├── Button.js
│ ├── Input.js
│ └── CourseCard.js
│
├── styles/
│ └── globals.css
│
├── ui-plan.md
├── tailwind.config.js
├── postcss.config.js
└── package.json


---

## 🎨 Styling Guidelines

- **Framework:** Tailwind CSS  
- **Color Theme:** Blue & Gray (educational and professional)  
- **Typography:** Sans-serif fonts for readability  
- **Spacing:** `p-4`, `m-4`, `rounded-lg`, `shadow-sm` for consistency  
- **Responsive Design:**  
  - `sm:` for mobile  
  - `md:` for tablet  
  - `lg:` for desktop  

---

## ✅ Expected Output
- The app runs locally (`npm run dev`) showing:
  - A responsive Navbar and Footer
  - A Login Page layout
  - A Dashboard Page layout
  - Reusable Button and Input components integrated

---
