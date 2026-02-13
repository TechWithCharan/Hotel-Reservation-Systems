# 🏨 Hotel Reservation System (Java + JDBC + MySQL)

This project is a **console-based Hotel Reservation System** built using **Core Java, JDBC, and MySQL**.
It allows users to **create, view, update, and delete hotel room reservations** through a simple menu-driven interface.

The project demonstrates how Java applications connect to databases and perform **CRUD operations** using **JDBC**.

---

## ✨ Features

* ➕ Reserve a new room with guest details
* 📋 View all current reservations in table format
* 🔍 Get room number using reservation ID and guest name
* ✏️ Update reservation information
* ❌ Delete an existing reservation
* 🗄️ MySQL database connectivity using JDBC

---

## 🛠️ Prerequisites

Ensure the following software is installed on your system:

* **Java JDK**
* **IntelliJ IDEA** (or any Java IDE)
* **MySQL Server**
* **MySQL Workbench**
* **Command Prompt / Terminal**
* **MySQL Connector/J**

Download MySQL Connector/J from:
https://dev.mysql.com/downloads/connector/j/

➡️ Choose **Platform Independent**, download the **ZIP file**, extract it, and use the **.jar file** inside your Java project libraries.

---

## ⚙️ Setup Steps Followed

1. Created a **Java project in IntelliJ IDEA** for JDBC practice.
2. Downloaded **MySQL Connector/J**, extracted the ZIP, and **added the JAR file as a library** in the project.
3. Created the **hotel_db database** and **reservations table** in MySQL Workbench.
4. Copied the **JDBC connection string** from MySQL Workbench and pasted it into the Java code.
5. Compiled and **successfully ran the program** from IntelliJ/terminal.

---

## 🗄️ Database Configuration

Run the following SQL commands in MySQL:

```sql
CREATE DATABASE hotel_db;

USE hotel_db;

CREATE TABLE reservations (
    reservation_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(255) NOT NULL,
    room_number INT NOT NULL,
    contact_number VARCHAR(255) NOT NULL,
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

---

## ▶️ How to Run the Project

1. Open the project in **IntelliJ IDEA**.
2. Make sure **MySQL Server is running** and the database/table are created.
3. Update database credentials in `HotelReservationSystem.java`:

```java
private static final String url = "jdbc:mysql://localhost:3306/hotel_db";
private static final String username = "root";
private static final String password = "your_password";
```

4. Run the main class:

```
HotelReservationSystem.java
```

5. Use the **console menu options** to perform reservation operations.

---

## 📂 Repository Structure

```
Hotel-Reservation-System/
 ├── HotelReservationSystem.java
 ├── hotel reservation outputs.pdf
 ├── mysql_connector_j_9_6_0.xml
 └── README.md
```

---

## 📸 Output

The file **hotel reservation outputs.pdf** contains:

* MySQL database and table creation
* Successful program execution
* Reservation insert, view, update, and delete operations

This confirms the project **works correctly**.

---

## 🎯 Learning Outcomes

* Understanding **JDBC connectivity in Java**
* Performing **CRUD operations in MySQL**
* Managing **user input in console applications**
* Integrating **Java with relational databases**

---

## 🚀 Future Improvements

* Use **PreparedStatement** to prevent SQL injection
* Add **GUI using Java Swing or JavaFX**
* Implement **room availability checking**
* Add **admin login authentication**

---

## 👨‍💻 Author

**Charan**
Java & MySQL Learner

GitHub: https://github.com/TechWithCharan

---

## 📄 License

This project is created for **educational purposes only**.
