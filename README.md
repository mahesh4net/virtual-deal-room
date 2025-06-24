# 🟢 Virtual Deal Room (VDR) – MERN Stack Application

This is a full-stack Virtual Deal Room platform that allows **Buyers** and **Sellers** to engage in secure deal negotiations, manage items, chat in real time, and handle payments — all within a streamlined dashboard interface.

## 🔗 Project Repositories

- **Frontend (React)**: [client-ui](https://github.com/mahesh4net/vdr-ui)
- **Backend (Node.js + Express)**: [vdr-server](https://github.com/mahesh4net/vdr-server)

---

## 📦 Tech Stack

- **Frontend**: React, Redux, React Router, Axios
- **Backend**: Node.js, Express.js, MongoDB (Mongoose)
- **Authentication**: JWT (stored in HTTP-only cookies)
- **Real-time Communication**: Socket.io (for chat)
- **Storage**: cloudinery (for images), MongoDB Atlas
- **Deployment**: Render.com (backend), Vercel (frontend)

---

## 👤 User Roles

1. **Buyer**
2. **Seller**
3. **Admin (incomplete)**

---

## 🚀 Key Features

### 🔐 Authentication
- Secure signup/login using JWT stored in HTTP-only cookies.
- Middleware-based route protection.
- Separate login flows for Buyers and Sellers.

### 🏠 Homepage
- **Buyers**: Browse all listed items, filter using search bar.
- **Sellers**: Create new listings directly from the homepage if logged in.

---

## 📊 Dashboard Overview

### Buyer Dashboard `/dashboard`

- **Sidebar Tabs**: Profile, Your Deals, Buy History, Chats, Notifications.
- **Your Deals**:
  - View all offers made by the buyer.
  - Negotiate (lower offer) anytime before acceptance.
  - Proceed to dummy payment on accepted deals.
- **Buy History**:
  - Displays all purchased items with total price and quantity.
- **Bought Items**:
  - Quick access list for all completed purchases.

---

### Seller Dashboard `/dashboard`

- **Sidebar Tabs**: Profile, Your Items, Buy History, Chats, Notifications.
- **Your Items**:
  - List of all items listed by the seller.
  - Clicking an item opens a dedicated item page.
- **Item Details Page**:
  - Split into `Overview`, `Deals`, and `Purchases` (tabbed via top menu).
  - View all incoming offers for that item and manage them.

---

## 🤝 Deal Management

- Sellers can accept, reject, or counter offers.
- Buyers can negotiate any pending offer.
- Status: `pending`, `accepted`, `rejected`, `completed`.

---

## 💳 Dummy Payment System

- Full-screen popup mimics real payment UI.
- Buyer can:
  - Choose quantity
  - Enter address, mobile, and card details (mock)
- Payment confirms deal and marks it as `completed`.

---

## 🔒 Security Best Practices

- JWT stored as HTTP-only cookie
- `.env` file excluded via `.gitignore`
- All protected routes require token validation via `verifyUser` middleware

---

## 🧠 Author

**Mahesh Kumar**  
[Portfolio](https://mahesh4net.github.io/portfolio/) | [GitHub](https://github.com/mahesh4net) | [LinkedIn](https://linkedin.com/in/mahesh4net)

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

