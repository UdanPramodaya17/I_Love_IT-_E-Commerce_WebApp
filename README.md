***

# 🛍️ I Love IT E-Commerce WebApp

I Love It is a full-stack MERN (MongoDB, Express, React, Node.js) e-commerce web application. It provides a complete online shopping experience, featuring secure user authentication, product management, a shopping cart, and integrated payment gateways.

## ✨ Key Features

* **Secure Authentication:** User registration and login protected by Bcrypt password hashing and JSON Web Tokens (JWT).
* **Role-Based Access:** Dedicated middleware for admin authorization to manage products and orders securely.
* **Product Management:** Full CRUD capabilities for products, complete with image uploading powered by Multer and Cloudinary.
* **Shopping Cart:** Persistent cart functionality allowing users to seamlessly add, remove, and manage items before checkout.
* **Payment Gateways:** Integrated with both Stripe and Razorpay for secure and flexible checkout options.
* **Modern & Responsive UI:** A fast, interactive frontend built with React 18, styled beautifully with Tailwind CSS, and optimized by Vite.
* **Notifications:** Real-time user feedback using React Toastify.

---

## 🛠️ Technology Stack

### Frontend
* **Framework:** React (`^18.3.1`) powered by Vite
* **Routing:** React Router DOM (`^6.26.1`)
* **Styling:** Tailwind CSS (`^3.4.10`) with PostCSS and Autoprefixer
* **HTTP Client:** Axios (`^1.7.4`)
* **Alerts:** React Toastify (`^10.0.5`)

### Backend
* **Runtime & Framework:** Node.js with Express (`^4.19.2`) using ES Modules
* **Database:** MongoDB with Mongoose (`^8.5.3`)
* **Authentication & Security:** JWT (`^9.0.2`), Bcrypt (`^5.1.1`), Validator (`^13.12.0`), and CORS (`^2.8.5`)
* **File Uploads:** Multer (`^1.4.5-lts.1`) and Cloudinary (`^2.4.0`)
* **Payments:** Stripe (`^16.8.0`) and Razorpay (`^2.9.4`)

---

## 📂 Project Structure

```text
I_Love_IT-full-stack/
├── backend/                  # Express.js backend API
│   ├── config/               # Database and third-party API configurations
│   ├── controllers/          # Route logic (user, product, cart, order)
│   ├── middleware/           # Auth, AdminAuth, and Multer middlewares
│   ├── models/               # Mongoose database schemas
│   ├── routes/               # Express API endpoints
│   ├── server.js             # Backend entry point
│   └── package.json          # Backend dependencies
└── frontend/                 # React.js frontend application
    ├── src/
    │   ├── assets/           # Images, icons, and static assets
    │   ├── components/       # Reusable UI elements (Navbar, Footer, ProductItem, etc.)
    │   ├── context/          # React Context (ShopContext) for state management
    │   ├── pages/            # Page views (Home, Cart, Login, Product, PlaceOrder, etc.)
    │   ├── App.jsx           # Main application component
    │   └── main.jsx          # React DOM entry point
    ├── vite.config.js        # Vite bundler configuration
    ├── tailwind.config.js    # Tailwind CSS configuration
    └── package.json          # Frontend dependencies
```

---

## 🚀 Getting Started

Follow these steps to get the project running on your local machine.

### Prerequisites
* [Node.js](https://nodejs.org/) (v16 or higher)
* [MongoDB](https://www.mongodb.com/) (Local instance or MongoDB Atlas)
* Accounts for Cloudinary, Stripe, and Razorpay (for full feature testing)

### 1. Clone the Repository
```bash
git clone https://github.com/UdanPramodaya17/I_Love_IT-_E-Commerce_WebApp.git
cd I_Love_IT-E-Commerce_WebApp/I_Love_IT-full-stack
```

### 2. Backend Setup
Navigate to the backend directory and install dependencies:
```bash
cd backend
npm install
```

Create a `.env` file in the `backend` folder and add your environment variables (e.g., `MONGO_URI`, `JWT_SECRET`, `CLOUDINARY_URL`, `STRIPE_SECRET_KEY`, `RAZORPAY_KEY_ID`, `RAZORPAY_KEY_SECRET`).

Start the backend development server:
```bash
npm run server
```

### 3. Frontend Setup
Open a new terminal window, navigate to the frontend directory, and install dependencies:
```bash
cd ../frontend
npm install
```

Start the frontend development server:
```bash
npm run dev
```

The frontend application should now be running on `http://localhost:5173` (or the port specified by Vite), communicating with your local backend API.

---

