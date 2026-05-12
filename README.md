# Ecommerce Backend

## Overview

This is the backend API for a full-stack ecommerce application built using Node.js, Express, Sequelize, and SQLite.

The backend provides:

* JWT Authentication
* Protected Routes
* User-specific Cart & Orders
* REST API Endpoints
* Sequelize ORM Integration

---

## Features

* User Registration & Login
* JWT Token Authentication
* Protected Middleware
* User-specific Cart System
* User-specific Orders
* Checkout Functionality
* Product APIs
* Delivery Options APIs

---

## Tech Stack

* Node.js
* Express.js
* Sequelize ORM
* SQLite
* JWT Authentication
* CORS

---

## Project Structure

```bash
routes/
middleware/
models/
config/
server.js
```

---

## Installation

### 1. Clone Repository

```bash
git clone YOUR_GITHUB_REPO_URL
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Create Environment Variables

Create a `.env` file in the root directory:

```env
JWT_SECRET=your_secret_key
PORT=7000
```

### 4. Start Development Server

```bash
npm run dev
```

---

## API Endpoints

### Authentication

```http
POST /api/users/register
POST /api/users/login
GET /api/users/me
```

### Products

```http
GET /api/products
```

### Cart

```http
GET /api/cart-items
POST /api/cart-items
PUT /api/cart-items/:id
DELETE /api/cart-items/:id
```

### Orders

```http
GET /api/orders
POST /api/orders
```

---

## Authentication

Protected routes require JWT token in headers:

```http
Authorization: Bearer YOUR_TOKEN
```

---

## Frontend

Connected with React + Vite frontend application.

---

## Troubleshooting

If you run into issues, check `TROUBLESHOOTING.md`.

---

## Future Improvements

* PostgreSQL Integration
* Payment Gateway
* Admin Dashboard
* Order Tracking
* Docker Deployment

---
