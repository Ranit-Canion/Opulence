# Opulence — Hotel Management (Admin + User Website)

[![Node.js](https://img.shields.io/badge/Node.js-18%2B-339933?logo=node.js&logoColor=white)](#)
[![Express](https://img.shields.io/badge/Express.js-4-000000?logo=express&logoColor=white)](#)
[![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-47A248?logo=mongodb&logoColor=white)](#)
[![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=black)](#)
[![Tailwind CSS](https://img.shields.io/badge/TailwindCSS-^3-06B6D4?logo=tailwindcss&logoColor=white)](#)
[![React Query](https://img.shields.io/badge/@tanstack%2Freact--query-FF4154?logo=reactquery&logoColor=white)](#)
[![JWT](https://img.shields.io/badge/Auth-JWT-000000?logo=jsonwebtokens&logoColor=white)](#)
[![Stripe](https://img.shields.io/badge/Payments-Stripe-635BFF?logo=stripe&logoColor=white)](#)

**Opulence** is a full-stack hotel management platform with a **public User Website** for booking rooms and a **role-based Admin Panel** (Admin & Employees) to manage rooms, bookings, guests, payments, and hotel settings. Features include **availability search**, **Stripe payments or pay-on-arrival**, **reviews**, **dashboards with charts**, and robust **JWT authentication**.

---

## ✨ Highlights

- **Authentication (JWT):** signup, login, logout, forgot/reset via email token, update password, delete profile.
- **User Website (Tailwind CSS):**
  - Check real-time availability by **date range (startDate–endDate)** and **guests**.
  - Filter & paginate rooms; **sort by price**.
  - Book via calendar (**date-fns**) with **Pay on Arrival** or **Stripe**.
  - View your bookings; post **reviews** for stayed rooms.
  - Manage profile (avatar, name, phone, etc.) and password.
- **Admin Panel (Styled Components):**
  - **Roles:** Admin, Employee (Employee can do all ops except employee management).
  - **Dashboard:** 
    - **Pie chart** for stays duration (# nights)
    - **Today’s Activity:** arriving / checked-in / checked-out
    - **Area chart**: sales over time
    - **Stats:** bookings, checked-in, checked-out, occupancy rate
  - **Rooms:** CRUD, pagination, filter (no discount / with discount), sort (price, capacity, name).
  - **Bookings:** confirm, **check-in**, **check-out**, delete, confirm **pay-on-arrival** payments; pagination; filter by status (unconfirmed, checked-in, checked-out); sort by amount/date.
  - **Hotel Settings:** Min/Max nights per booking, Max guests/booking, Breakfast price.
  - **Employees (Admin only):** create/delete employee accounts.
  - Admin profile & password management.

> Charts are implemented with **Recharts**.

---

## 🧱 Tech Stack

- **Frontend (User Website):** React, React Router, Tailwind CSS, @tanstack/react-query, date-fns, Stripe.js
- **Frontend (Admin Panel):** React, React Router, **Styled Components**, @tanstack/react-query, Recharts
- **Backend:** Node.js, Express.js, MongoDB (Mongoose), Nodemailer, JWT, Multer (optional for avatar), Stripe SDK
- **Utilities:** date-fns, bcrypt, helmet, cors, express-rate-limit
- **Payments:** Stripe (Card payments); Pay on arrival toggle

---

## 📸 Screenshots (add yours)

```txt
docs/
 └─ screenshots/
    ├─ user-home.png
    ├─ user-room-details.png
    ├─ user-checkout.png
    ├─ admin-dashboard.png
    ├─ admin-rooms.png
    ├─ admin-bookings.png
    └─ admin-settings.png
