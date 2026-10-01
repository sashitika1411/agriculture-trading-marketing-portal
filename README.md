# 🌾 Agriculture Marketing and Trading Portal with Auction System

A full-stack web application designed to provide a digital platform for **agricultural product marketing and trading**. The system connects farmers and buyers, allowing agricultural products to be listed, viewed, and traded through an online platform.

The project also includes an **auction system** to support auction-based trading of agricultural products.

---

## 📌 Project Overview

Traditional agricultural trading can involve multiple intermediaries and limited access to buyers. This project aims to provide a digital marketplace where farmers can showcase their agricultural products and buyers can discover and purchase products through an online platform.

The application is developed using **React.js for the frontend, Spring Boot for the backend, and MySQL for database management**.

---

## 🎯 Objectives

* Provide an online marketplace for agricultural products.
* Help farmers list and manage their products digitally.
* Allow buyers to browse available agricultural products.
* Support agricultural product trading.
* Provide an auction mechanism for selected products.
* Maintain product, user, order, and auction information.
* Reduce dependency on traditional trading intermediaries.

---

## ✨ Key Features

### 👨‍🌾 Farmer

* Farmer registration and login
* Add agricultural products
* Manage product information
* View listed products
* Manage trading-related information

### 🛒 Buyer

* Buyer registration and login
* Browse agricultural products
* View product details
* Purchase agricultural products
* View order information

### 🔨 Auction System

* Create auctions for agricultural products
* Display auction information
* Allow buyers to participate in bidding
* Manage auction-related information

### 📦 Order Management

* Create orders
* Store order details
* View order information
* Manage order status

### 👤 User Management

* User registration
* User information management
* Farmer and buyer roles

---

## 🏗️ System Architecture

```text
                  ┌──────────────────────┐
                  │      React.js        │
                  │      Frontend        │
                  └──────────┬───────────┘
                             │
                             │ REST API
                             ▼
                  ┌──────────────────────┐
                  │     Spring Boot      │
                  │       Backend        │
                  ├──────────────────────┤
                  │ Controllers           │
                  │ Services              │
                  │ Repositories          │
                  │ Entities / Models     │
                  └──────────┬───────────┘
                             │
                             │ JPA / Hibernate
                             ▼
                  ┌──────────────────────┐
                  │        MySQL         │
                  │       Database       │
                  └──────────────────────┘
```

---

## 🛠️ Technologies Used

### Frontend

* React.js
* JavaScript
* HTML5
* CSS3

### Backend

* Java
* Spring Boot
* Spring Data JPA
* Hibernate
* REST API

### Database

* MySQL

### Build Tool

* Maven

### Tools

* Visual Studio Code
* Git
* GitHub
* Node.js
* npm

---

## 📂 Project Structure

```text
agriculture-trading-marketing-portal/
│
├── agri-frontend/
│   ├── public/
│   ├── src/
│   ├── package.json
│   └── ...
│
├── src/
│   └── main/
│       ├── java/
│       │   └── com/
│       │       └── agriportal/
│       │           ├── controller/
│       │           ├── model/
│       │           ├── repository/
│       │           ├── service/
│       │           └── ...
│       │
│       └── resources/
│
├── pom.xml
├── .gitignore
└── README.md
```

---

## 🗄️ Database

The application uses **MySQL** as the database.

The database stores information related to:

* Users
* Agricultural products
* Orders
* Auctions

Create the database using:

```sql
CREATE DATABASE agri_db;
```

> Database credentials are not included in this repository for security reasons.

---

## 🚀 How to Run the Project

### Prerequisites

Install the following before running the project:

* Java JDK
* Maven
* Node.js
* npm
* MySQL
* Git

---

## ⚙️ Backend Setup

### 1. Clone the repository

```bash
git clone https://github.com/sashitika1411/agriculture-trading-marketing-portal.git
```

### 2. Navigate to the project

```bash
cd agriculture-trading-marketing-portal
```

### 3. Create the MySQL database

```sql
CREATE DATABASE agri_db;
```

### 4. Configure the database

Create your local Spring Boot configuration and provide your own MySQL username and password.

**Do not commit database credentials to GitHub.**

### 5. Run the Spring Boot application

On Windows:

```bash
mvnw.cmd spring-boot:run
```

Or using Maven:

```bash
mvn spring-boot:run
```

The backend will run on:

```text
http://localhost:8080
```

---

## 💻 Frontend Setup

Open another terminal and navigate to the frontend:

```bash
cd agri-frontend
```

Install dependencies:

```bash
npm install
```

Start the frontend:

```bash
npm run dev
```

The terminal will display the local frontend URL.

---

## 🔗 Application Communication

The React frontend communicates with the Spring Boot backend through **REST APIs**.

```text
React.js
   │
   │ HTTP Requests
   ▼
Spring Boot REST API
   │
   ▼
MySQL Database
```

---

## 🔐 Security

Sensitive configuration files are excluded from GitHub using `.gitignore`.

For example:

```text
.env
.env.*
src/main/resources/application.properties
```

This helps prevent sensitive information such as database passwords and API credentials from being committed to the repository.

---

## 📊 Main Modules

| Module             | Description                                    |
| ------------------ | ---------------------------------------------- |
| User Management    | Handles user registration and user information |
| Product Management | Manages agricultural product information       |
| Order Management   | Handles buyer orders                           |
| Auction Management | Supports auction-based trading                 |
| Frontend           | Provides the web interface                     |
| Database           | Stores application data                        |

---

## 🔮 Future Enhancements

* Online payment integration
* Real-time auction bidding
* Email notifications
* SMS notifications
* Product image upload
* Advanced search and filtering
* Farmer dashboard
* Buyer dashboard
* Order tracking
* Product ratings and reviews
* Mobile application
* Enhanced authentication and authorization

---

## 🎓 Project Purpose

This project was developed as an academic and practical full-stack development project to demonstrate the use of **Java, Spring Boot, React.js, REST APIs, MySQL, and Git/GitHub** in building an agricultural trading platform.

---

## 👩‍💻 Developer

**Sashitika Ravikumar**

GitHub: [sashitika1411](https://github.com/sashitika1411)

---

## 📄 License

This project currently does not include an open-source license.

