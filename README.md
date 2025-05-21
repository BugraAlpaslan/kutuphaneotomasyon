
---

# 📚 JavaFX Library Management System

A modern **desktop application** built using **JavaFX** to manage core library operations such as book inventory, member registration, and lending transactions. The app features an intuitive GUI for both admins and members.

![JavaFX UI Demo](https://via.placeholder.com/800x500?text=JavaFX+Library+Management+UI)
*Replace with actual UI screenshots.*

---

## ✨ Features

### 📘 Book Management

* Add, edit, delete book records (ISBN, title, author, category).
* Automatically track book availability.

### 🧑‍💼 Member Management

* Register new members.
* View member borrowing history and details.

### 🔁 Borrowing System

* Borrow and return books.
* Track due dates and return status.

### 🖥️ User Interface

* Role-based login (Admin/Member).
* Clean and responsive dashboard.
* Book search and filtering.

---

## 🛠️ Tech Stack

| Layer        | Tech                            |
| ------------ | ------------------------------- |
| Language     | Java 17+                        |
| UI Framework | JavaFX 20 (FXML, Scene Builder) |
| Database     | MySQL                           |
| Connectivity | JDBC                            |
| IDE          | IntelliJ IDEA / Eclipse         |

---

## 🚀 Getting Started

### 1. Prerequisites

* Java 17 or newer.
* JavaFX SDK .
* MySQL Server.
* Scene Builder (for FXML editing).

### 2. Database Setup

* Import the provided `database.sql` file into MySQL.
* Update credentials in `DBConnector.java`:

  ```java
  String DB_URL = "jdbc:mysql://localhost:3306/library_db";
  String USER = "root";
  String PASS = "your_password";
  ```

### 3. IDE Configuration

If using IntelliJ/Eclipse, set VM options:

```sh
--module-path /path/to/javafx-sdk-20/lib --add-modules javafx.controls,javafx.fxml
```

#### Maven Dependency (Optional)

```xml
<dependency>
  <groupId>org.openjfx</groupId>
  <artifactId>javafx-controls</artifactId>
  <version>20</version>
</dependency>
```

### 4. Run the App

* Main class: `src/main/java/com/bugraalpaslan/MainApplication.java`
* **Default Login** (optional): `Admin / Admin123`

---



## 🔧 Customization Tips

* Modify UI via `.fxml` files using **Scene Builder**.
* Adjust themes with `style.css`:

  ```css
  .button {
    -fx-background-color: #4CAF50;
  }
  ```

---

## 🤝 Contribution Guide

### Ideas for Enhancement

* Generate **PDF reports** (e.g., using Apache PDFBox).
* Implement **dark/light mode**.
* Add **email notifications** for due dates.

### Reporting Issues

Please open an issue on the [GitHub Issues](../../issues) tab with relevant details and screenshots.

---



