# Sports Item Shop

Repository: [harshitch161/Sports-Item-Shop](https://github.com/harshitch161/Sports-Item-Shop)

---

## Overview

Sports Item Shop is a Java-based desktop application designed to provide a user-friendly interface for shopping various sports equipment. Developed in NetBeans IDE using Java (100%),
it leverages MySQL for robust, high-performance database management. This project demonstrates proficiency in building full-featured CRUD applications integrated with relational databases.

---

## Features

- **Product Catalog:** Browse, view, and search sports items by category, price, or name.
- **User Registration & Authentication:** Secure login/signup functionality for buyers and admins.
- **Inventory Management:** Admins can add, edit, and delete products; stock tracking.
- **Shopping Cart:** Users can add sports items to a cart and proceed to checkout.
- **Order Processing:** Store and manage user orders and purchase history.
- **Reports & Analytics:** Basic sales and inventory reports for admin users.
- **GUI:** Intuitive desktop user interface built with Java Swing (NetBeans GUI builder).
- **Database Integration:** All application data stored in MySQL, designed for scalability.

---

## Technology Stack

- **Language:** Java (100%), object-oriented programming, JDBC for database connectivity
- **IDE:** NetBeans
- **Database:** MySQL (tables for users, products, orders, cart, etc.)
- **GUI:** Swing components (JFrame, JDialog, JTable, JComboBox, etc.)
- **Architecture:** Layered (GUI, business logic, data access)

---

## Setup Instructions

### Prerequisites

- [NetBeans IDE](https://netbeans.apache.org/) (recommended for best experience)
- [Java JDK 8+](https://www.oracle.com/java/technologies/downloads/)
- [MySQL Server](https://dev.mysql.com/downloads/mysql/)

### Database Configuration

1. **Create the database:**
   - Open MySQL and run the provided SQL script (`database.sql`) or create a database named `sports_shop`.
2. **Configure tables:**
   - Create tables for `users`, `products`, `orders`, `cart`, etc.
   - Example:
     ```sql
     CREATE TABLE users (
         id INT PRIMARY KEY AUTO_INCREMENT,
         username VARCHAR(50),
         password VARCHAR(255),
         role VARCHAR(20)
     );
     ```
   - Adjust according to provided schema in the repository (add your script here if available).

3. **Set MySQL connection settings in code:**
   - Locate the database connection class (typically `DBConnection.java` or similar), and update:
     ```
     DB_URL = "jdbc:mysql://localhost:3306/sports_shop";
     DB_USER = "root";
     DB_PASSWORD = "your_mysql_password";
     ```

### Running the Project

1. **Open in NetBeans**
   - Clone the repository:
     ```
     git clone https://github.com/harshitch161/Sports-Item-Shop.git
     ```
   - Open the project folder in NetBeans.

2. **Add Libraries**
   - Right-click project > Properties > Libraries > Add JAR/Folder.
   - Add MySQL JDBC Connector JAR.

3. **Build and Run**
   - Clean and build the project.
   - Press F6 or click the "Run" button.

4. **Login/Signup**
   - Use default admin credentials (if provided) to access the admin panel, or register as a new user.

---

## Project Structure

```
Sports-Item-Shop/
├── src/
│   ├── main/ (Java source files)
│   │   ├── gui/ (Swing UI classes)
│   │   ├── dao/ (Database access objects)
│   │   ├── model/ (Entity/data classes)
│   │   └── util/ (Helper classes, DBConfig)
│   └── resources/ (SQL scripts, images)
├── database.sql (sample DB script)
├── README.md
```

---

## Contribution

PRs and suggestions are welcome!  
If you spot bugs or have improvement ideas, please open an issue or a pull request with detailed info.

---

## Author

**Harshit Chaurasia**  
[GitHub Profile](https://github.com/harshitch161)

---
