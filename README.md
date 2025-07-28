# Products Management API

A RESTful API for managing products built with Node.js and Express.js.

## Features

- ✅ Get all products
- ✅ Get product by ID
- ✅ Create new product
- ✅ Update existing product
- ✅ Delete product

## Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd PRODUCTS_MANAGEMENT
```

2. Install dependencies:
```bash
npm install
```

3. Start the server:
```bash
npm start
```

Or for development with auto-restart:
```bash
npm run dev
```

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/products` | Get all products |
| GET | `/products/:id` | Get product by ID |
| POST | `/products` | Create new product |
| PUT | `/products/:id` | Update product by ID |
| DELETE | `/products/:id` | Delete product by ID |

## Example Usage

### Get all products
```http
GET http://localhost:3000/products
```

### Create a new product
```http
POST http://localhost:3000/products
Content-Type: application/json

{
  "productName": "New Product",
  "price": 1500
}
```

### Update a product
```http
PUT http://localhost:3000/products/1
Content-Type: application/json

{
  "productName": "Updated Product",
  "price": 2000
}
```

### Delete a product
```http
DELETE http://localhost:3000/products/1
```

## Project Structure

```
PRODUCTS_MANAGEMENT/
├── controllers/
│   └── products.controllers.js
├── data/
│   └── products.js
├── routes/
│   └── products.routes.js
├── server.js
├── package.json
└── README.md
```

## Technologies Used

- Node.js
- Express.js
- Nodemon (for development)

## Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).
