# Fake Ecommerce API

Free REST API for learning and portfolio projects. No auth needed.

## Base URL
https://mock-ecommerce-api-g93f.onrender.com/api/v1

## Endpoints

### Products
GET /products - Get all products
GET /products/:id - Get single product
GET /products?category=Mobile - Filter by category
GET /products?brand=Apple - Filter by brand
GET /products?_sort=price&_order=asc - Sort by price
GET /products?q=iphone - Search products
GET /products?_page=1&_limit=5 - Pagination

### Users
GET /users
GET /users/:id

### Cart
GET /cart?userId=1 - Get user cart
POST /cart - Add to cart

### Orders
GET /orders?userId=1 - Get user orders

## Example
fetch('https://mock-ecommerce-api-g93f.onrender.com//api/v1/products')
  .then(res => res.json())
  .then(data => console.log(data))
