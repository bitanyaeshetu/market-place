Et_merkato - E-commerce Platform for Merkato Market
Et_merkato is an online marketplace designed to bridge the gap between local vendors at Merkato and their potential customers. The platform allows customers to browse products, place orders, and make secure payments, while also providing vendors with a system to manage their inventory, process orders, and gain visibility for their businesses.

Table of Contents
Project Description
Core Features and Functionality
API Endpoints
Tools and Libraries
Installation and Setup
Usage
Contributing
License
Project Description
Et_merkato is an e-commerce platform designed to bring together local vendors and customers in the Merkato market area. The platform offers a seamless shopping experience with product listings, order management, payment integrations, and vendor dashboards. The goal is to create a marketplace that serves both customers and vendors in a simple and efficient way.

Core Features and Functionality
User Authentication:

Sign up and login functionality for both customers and vendors.
Secure authentication using JWT (JSON Web Tokens).
Product Listings:

Vendors can list products with detailed descriptions, prices, and images.
Customers can view and browse product listings.
Search and Filtering:

Customers can search for products and filter them by categories, price range, and popularity.
Shopping Cart:

Customers can add products to the shopping cart and proceed to checkout.
Order Management:

Customers can view their order history and track the status of their orders.
Vendors can manage their orders and update statuses.
Vendor Dashboard:

Vendors can manage their inventory, view orders, and analyze sales performance.
Payment Integration:

Integration with payment systems such as Telebirr, M-Birr, or Stripe/PayPal.
Shipping/Delivery:

Integration with local and international shipping services.
API Endpoints
User Authentication:
POST /users/signup: User registration (Customer/Vendor).
POST /users/login: User login (Customer/Vendor).
Products:
GET /products: Retrieve a list of all products.
GET /products/{id}: Retrieve product details by product ID.
Orders:
POST /orders: Create a new order.
GET /orders/{order_id}: Retrieve order details by order ID.
PUT /orders/{order_id}/status: Update the status of an order (e.g., shipped, delivered).
Payment:
POST /payment: Process a payment for an order.
Tools and Libraries
Django: Web framework for building the backend and API.
Django REST Framework: A powerful toolkit to build RESTful APIs in Django.
PostgreSQL: Database for storing users, products, and orders.
Celery: For background task management (e.g., order processing).
Stripe/PayPal/Telebirr: For payment gateway integration.
Docker: Containerization for easier deployment.
Gunicorn: WSGI HTTP server for running the Django app in production.
Installation and Setup
Prerequisites
Python 3.8 or higher
pip (Python package installer)
PostgreSQL (for local development, you can use SQLite as an alternative)
git clone https://github.com/bitanyaeshetu/market place