# Vinayaga Bakery - Backend API

A robust **RESTful API** for Vinayaga Bakery Point of Sale (POS) system built with **Node.js**, **Express.js**, and **MongoDB**. This backend provides secure, scalable API endpoints for bakery operations including product management, order processing, and inventory tracking.

## 🎯 Features

- **RESTful API Architecture** - Clean and scalable API design
- **CRUD Operations** - Complete Create, Read, Update, Delete functionality for products and orders
- **MongoDB Integration** - NoSQL database for flexible data management
- **Authentication & Authorization** - JWT-based secure authentication
- **Error Handling** - Comprehensive error management and validation
- **Security** - Helmet.js for HTTP headers security
- **CORS Support** - Cross-Origin Resource Sharing enabled for frontend integration
- **Logging** - Morgan middleware for API request/response logging
- **Environment Configuration** - Dotenv for secure environment variable management

## 🛠️ Tech Stack

| Technology | Version | Purpose |
|---|---|---|
| Node.js | LTS | JavaScript Runtime |
| Express.js | ^4.19.2 | Web Framework |
| MongoDB | Latest | NoSQL Database |
| Mongoose | ^8.10.0 | MongoDB ODM |
| JWT | - | Authentication |
| Helmet | ^7.1.0 | Security Headers |
| CORS | ^2.8.5 | Cross-Origin Support |
| Morgan | ^1.10.0 | HTTP Logging |
| Dotenv | ^16.4.5 | Environment Config |

## 📦 Installation

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (Local or Atlas)
- npm or yarn package manager

### Steps

```bash
# Clone the repository
git clone https://github.com/vijay-890/vinayaga-bakery-backend.git

# Navigate to project directory
cd vinayaga-bakery-backend

# Install dependencies
npm install
```

## ⚙️ Environment Setup

Create a `.env` file in the root directory with the following variables:

```env
PORT=5000
NODE_ENV=development
MONGODB_URI=mongodb://localhost:27017/vinayaga-bakery
JWT_SECRET=your_jwt_secret_key_here
JWT_EXPIRE=7d
CORS_ORIGIN=http://localhost:3000
```

## 🚀 Running the Server

```bash
# Development mode (with hot reload using nodemon)
npm run dev

# Production mode
npm start
```

Server will start at: `http://localhost:5000`

## 📋 API Endpoints

### Products
- `GET /api/products` - Fetch all products
- `GET /api/products/:id` - Fetch product by ID
- `POST /api/products` - Create new product
- `PUT /api/products/:id` - Update product
- `DELETE /api/products/:id` - Delete product

### Orders
- `GET /api/orders` - Fetch all orders
- `GET /api/orders/:id` - Fetch order by ID
- `POST /api/orders` - Create new order
- `PUT /api/orders/:id` - Update order status
- `DELETE /api/orders/:id` - Delete order

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout

## 📁 Project Structure

```
vinayaga-bakery-backend/
├── server.js              # Entry point
├── package.json           # Dependencies
├── .env.example           # Environment template
├── routes/                # API route handlers
│   ├── products.js
│   ├── orders.js
│   └── auth.js
├── models/                # MongoDB schemas
│   ├── Product.js
│   ├── Order.js
│   └── User.js
├── controllers/           # Business logic
├── middleware/            # Custom middleware
│   ├── auth.js
│   └── errorHandler.js
└── config/                # Configuration files
```

## 🔐 Security Features

- **Helmet.js** - Protects against common web vulnerabilities
- **CORS Configuration** - Restricts API access to authorized origins
- **JWT Authentication** - Secure token-based authentication
- **Environment Variables** - Sensitive data protection
- **Input Validation** - Request validation middleware
- **Error Handling** - Safe error responses without exposing sensitive info

## 🧪 Testing

```bash
# Test API endpoints (using Postman or cURL)
curl http://localhost:5000/api/products
```

## 📚 API Documentation

For detailed API documentation with request/response examples, refer to the Postman collection:
[Add Postman Collection Link]

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 Commit Message Guidelines

- Use descriptive commit messages
- Format: `type(scope): description`
- Examples:
  - `feat(products): add product filtering`
  - `fix(orders): handle null order status`
  - `docs(api): update endpoint documentation`

## 🐛 Known Issues

- [Add any known issues or limitations]

## 🚧 Future Enhancements

- [ ] Implement caching with Redis
- [ ] Add unit and integration tests
- [ ] Implement API rate limiting
- [ ] Add WebSocket support for real-time updates
- [ ] Deploy to cloud (AWS/Heroku)
- [ ] Add Swagger API documentation

## 📄 License

MIT License - See LICENSE file for details

## 👨‍💻 Author

**V. Vijay**
- GitHub: [@vijay-890](https://github.com/vijay-890)
- Email: vijayvijay23747@gmail.com
- LinkedIn: [vijay-v-457692325](https://www.linkedin.com/in/vijay-v-457692325)

## 📞 Support

For issues, questions, or suggestions:
1. Open an issue on GitHub
2. Contact via email: vijayvijay23747@gmail.com
3. Check existing documentation

## 🙏 Acknowledgments

- Built as part of MERN Stack development course
- Inspired by modern bakery management systems
- Developed with passion for clean code and best practices

---

**Last Updated:** 2026-04-05 18:33:13
**Status:** Active Development ✅