# E-Commerce Platform

<p align="center">
  <strong>A full-stack e-commerce solution with modern tech stack</strong>
</p>

## Overview

This is a production-ready e-commerce platform built with React, Node.js, Express, and MongoDB. It provides a complete shopping experience including user authentication, product management, shopping cart, payment processing, and admin dashboard.

## Features

✅ **User Management**
- User registration and authentication
- JWT-based authorization
- User profile management
- Order history tracking

✅ **Product Management**
- Dynamic product catalog
- Advanced filtering and search
- Product ratings and reviews
- Image uploads

✅ **Shopping Cart**
- Add/remove products
- Quantity management
- Real-time cart updates
- Persistent storage

✅ **Payment Integration**
- Stripe payment gateway
- Secure transactions
- Multiple payment methods
- Order confirmation emails

✅ **Admin Dashboard**
- Product management
- Order tracking
- User management
- Sales analytics and reports

## Tech Stack

### Frontend
- **React 18** - UI library
- **Redux Toolkit** - State management
- **Axios** - HTTP client
- **Tailwind CSS** - Styling
- **React Router v6** - Navigation

### Backend
- **Node.js** - Runtime
- **Express.js** - Web framework
- **MongoDB** - Database
- **Mongoose** - ODM
- **JWT** - Authentication
- **Stripe API** - Payments

## Project Structure

```
ecommerce-platform/
├── client/                 # React frontend
│   ├── public/
│   ├── src/
│   │   ├── components/     # Reusable components
│   │   ├── pages/          # Page components
│   │   ├── redux/          # Redux slices
│   │   ├── services/       # API calls
│   │   ├── styles/         # CSS files
│   │   └── App.jsx
│   └── package.json
│
├── server/                 # Express backend
│   ├── models/             # MongoDB models
│   ├── routes/             # API routes
│   ├── controllers/        # Route handlers
│   ├── middleware/         # Custom middleware
│   ├── config/             # Configuration
│   ├── utils/              # Helper functions
│   └── server.js
│
├── .gitignore
├── .env.example
└── README.md
```

## Installation

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- Git

### Backend Setup

1. Clone the repository
```bash
git clone https://github.com/nayaabhussain871-web/ecommerce-platform.git
cd ecommerce-platform/server
```

2. Install dependencies
```bash
npm install
```

3. Create `.env` file
```bash
cp .env.example .env
```

4. Configure environment variables
```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/ecommerce
JWT_SECRET=your_jwt_secret_key
STRIPE_SECRET_KEY=your_stripe_secret_key
NODE_ENV=development
```

5. Start the server
```bash
npm start
```

### Frontend Setup

1. Navigate to client directory
```bash
cd ../client
```

2. Install dependencies
```bash
npm install
```

3. Create `.env` file
```bash
REACT_APP_API_URL=http://localhost:5000/api
```

4. Start the development server
```bash
npm start
```

## API Documentation

### Authentication Endpoints
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout
- `GET /api/auth/profile` - Get user profile

### Product Endpoints
- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get product by ID
- `POST /api/products` - Create product (Admin)
- `PUT /api/products/:id` - Update product (Admin)
- `DELETE /api/products/:id` - Delete product (Admin)

### Order Endpoints
- `GET /api/orders` - Get user orders
- `POST /api/orders` - Create order
- `GET /api/orders/:id` - Get order details
- `PUT /api/orders/:id` - Update order status (Admin)

## Usage

### Customer Flow
1. Register/Login to your account
2. Browse products and use filters
3. Add items to cart
4. Proceed to checkout
5. Make payment via Stripe
6. View order confirmation and history

### Admin Flow
1. Login with admin credentials
2. Access admin dashboard
3. Manage products (Create, Update, Delete)
4. View and manage orders
5. Track sales and analytics

## Development

### Available Scripts

**Server:**
```bash
npm start           # Start development server
npm run dev         # Start with nodemon
npm test            # Run tests
```

**Client:**
```bash
npm start           # Start development server
npm build           # Build for production
npm test            # Run tests
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

MIT License - see LICENSE file for details

## Contact

For questions or suggestions, please open an issue or contact me.

---

**Last Updated:** November 2025
