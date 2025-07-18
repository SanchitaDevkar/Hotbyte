HotByte – Online Food Ordering System

HotByte is a full-stack web application that allows users to conveniently browse restaurants, manage their cart, and place food orders. The platform supports role-based access for users, restaurant owners, and admins. Built using **Spring Boot (Java)** for the backend and **Angular** for the frontend, it is secure, scalable, and ideal for learning or deployment in real-world scenarios.

---

## 🔎 Overview

This system is designed to simulate a real-world online food ordering platform where:

- Users:can register, explore restaurants, add food items to their cart, and place orders.
- Restaurants:can manage their menu and view order requests.
- Admins:can monitor the entire system and perform managerial actions.

---

## 📁 Project Structure

CompleteProject/
│
├── HotByte-frontend/ # Angular Frontend
│ └── HotByteFrontend/
│
├── Hotbyte-Backend/ # Spring Boot Backend
│ └── Hotbyte-Backend/
│
└── Database/ # MySQL SQL Scripts
├── demo_user.sql
├── demo_admin.sql
├── demo_restaurant.sql
├── demo_menu.sql
├── demo_cart.sql
├── demo_cart_item.sql
├── demo_orders.sql
└── demo_order_item.sql

---

## 🚀 Key Features

### 👤 User
- Register and login with JWT authentication
- Browse menu with search and filter
- Add/remove items to cart
- Place orders and view order history

### 🍴 Restaurant
- Manage menu items (Add/Edit/Delete)
- Categorize food (e.g., Starters, Main Course, Desserts)
- Update item availability
- Track and update order status

### 🛡️ Admin
- View and manage users, restaurants, and orders
- Block/unblock restaurants and users
- Full access to system logs and records

---

## 🧰 Tech Stack

| Layer         | Technology                      |
|---------------|----------------------------------|
| Frontend      | Angular 16+                      |
| Backend       | Spring Boot (Java)               |
| Database      | MySQL                            |
| ORM           | Spring Data JPA (Hibernate)      |
| Security      | Spring Security + JWT            |
| Styling       | Bootstrap                        |
| Build Tool    | Maven                            |
| Forms         | Reactive Forms (Angular)         |

---

## 🛠️ Setup Instructions

### 1️⃣ Clone the Project

```bash
git clone https://github.com/yourusername/Hotbyte.git
cd CompleteProject
2️⃣ Backend Setup (Spring Boot)
Navigate to:

bash
cd Hotbyte-Backend/Hotbyte-Backend
Update application.properties:

properties
spring.datasource.url=jdbc:mysql://localhost:3306/Database
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
jwt.secret=your_jwt_secret_key
Run the project:

bash
./mvnw spring-boot:run
Backend will start at http://localhost:8080.

3️⃣ Frontend Setup (Angular)
Navigate to:

bash
cd HotByte-frontend/HotByteFrontend
Install dependencies:

bash
npm install
Start the Angular app:

bash
ng serve
Frontend will be available at http://localhost:4200.

4️⃣ MySQL Database Setup
Create a database:

sql
CREATE DATABASE Database;
Import the SQL files from the Database/ folder in this order:

demo_user.sql

demo_admin.sql

demo_restaurant.sql

demo_menu.sql

demo_cart.sql

demo_cart_item.sql

demo_orders.sql

demo_order_item.sql

🔐 Default Login Credentials
Admin
makefile
Email: admin@hotbyte.com
Password: admin123
You can add restaurant and user credentials via the database or registration flow.

🧪 Roles and Access
Role	Access To
ROLE_USER	Menu, cart, order placement
ROLE_RESTAURANT	Menu and order management
ROLE_ADMIN	System-wide access and controls

🌟 Future Enhancements
Payment gateway integration (e.g., Razorpay)

Delivery tracking system

Review & rating system

Docker support for deployment

Notification system (email/SMS)

 Author
Sanchita Devkar
1. project name:Hotbyte
2. username :SanchitaDevkar
3. email id:sanchita.devkar21@pccoepune.org

