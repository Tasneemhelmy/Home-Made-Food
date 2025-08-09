Homemade Food API
Backend system for a platform connecting users with home-made-food chefs to order and manage meals.

Overview
A comprehensive backend service enabling users to browse, order, and review home-made meals while allowing chefs to manage their listings and track orders.
Includes secure authentication, role-based access control, and OTP-based password recovery.
--------------------------------------------------------------------------------------------------------------------------------------------------------------
Key Features
Authentication & Security

User registration, login, logout with JWT

OTP-based password reset

Role-based access: Users, Chefs, Admins

Social login via Google & Facebook

User Functionalities

View meals, add to cart, checkout

Manage delivery addresses

Follow chefs & view followed chefs

Review and rate meals

Personalized meal recommendations based on order history

Search meals by image similarity

Chef Functionalities

Add, edit, and manage meals with image uploads to Cloudinary

Receive and update orders’ status

View followed users

Advanced Features

Image-based meal search

Email notifications via Nodemailer

Automatic total price calculation for orders
-------------------------------------------------------------------------------------------------------------------------------------------------------------
Use Cases
User flow – Sign up, log in, browse meals, add to cart, checkout, review meals.

Password reset – Reset password with OTP via email.

Image Search – Upload a food image to find similar meals.

Recommendations – View meals suggested from previous orders.

Chef flow – Add meals, receive orders, update order statuses.
----------------------------------------------------------------------------------------------------------------------------------------------------------------

API Endpoints (Highlights)
🔐 Auth
POST /auth/login – Login

PATCH /auth/verify-email – Verify email

POST /auth/send-otp – Send OTP for password reset

POST /auth/signup-user – Register as User

POST /auth/signup-chef – Register as Chef

📍 Address (User)
POST /address – Add address

GET /address – Get all addresses

🍽️ Meals
GET /meals – Get all meals

POST /meals/favorite – Add to favorites

🛒 Cart
POST /cart – Add meal to cart

PUT /cart/checkout – Checkout cart

📦 Orders
GET /orders/user – Get user orders

PUT /orders/status/:id – Update order status

📝 Reviews
POST /reviews – Add or update review

🔍 Search & Recommendations
POST /similar – Search by image

POST /get-recommended-meals – Personalized recommendations
----------------------------------------------------------------------------------------------------------------------------------------------------------------
Tech Stack
Backend Framework: Node.js + Express.js

Database: MongoDB

Authentication: JWT, OTP

File Storage: Cloudinary

Email Service: Nodemailer

Search & Recommendations: Image similarity + history-based suggestions
------------------------------------------------------------------------------------------------------------------------------------------------------------------
Team
Toaa Mahmoud

Khaled Saeed

Tasneem Helmy

