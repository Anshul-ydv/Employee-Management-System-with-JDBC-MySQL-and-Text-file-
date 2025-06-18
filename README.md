
# 🚀 Employee Management System

![Java](https://img.shields.io/badge/Java-%231572B6.svg?style=for-the-badge&logo=java&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
![JDBC](https://img.shields.io/badge/JDBC-Connector-blue?style=for-the-badge)

A **console-based Employee Management System** built using **Java**, **JDBC**, and **MySQL**, with backup capabilities using **text files**. This project provides basic employee CRUD operations and can serve as a strong foundation for beginners learning Java database programming.

---

## 📚 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Setup Instructions](#-setup-instructions)
- [Project Structure](#-project-structure)
- [Contributing](#-contributing)
- [License](#-license)
- [Author](#-author)

---

## ✨ Features

✅ Add new employees  
✅ View all employee records  
✅ Update employee details  
✅ Delete employee records  
✅ Search employees by ID  
✅ Store data in MySQL & backup in text files  
✅ Clean, modular OOP-based code  

---

## 🛠 Tech Stack

| Layer           | Technology                  |
|-----------------|-----------------------------|
| Language        | Java                        |
| Database        | MySQL                       |
| DB Connector    | JDBC (MySQL Connector/J)    |
| File Storage    | `.txt` text files           |
| Interface       | Console-based UI            |

---

## 🔧 Setup Instructions

### 1. Prerequisites

- Java JDK 8 or above
- MySQL Server
- Any Java IDE (e.g., IntelliJ, Eclipse) or CLI
- MySQL Connector/J `.jar` file

### 2. Clone the Repository

```bash
git clone https://github.com/Anshul-ydv/Employee-Management-System.git
cd Employee-Management-System
````

### 3. Configure MySQL

```sql
CREATE DATABASE employee_db;

USE employee_db;

CREATE TABLE employee (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    department VARCHAR(100),
    salary DOUBLE
);
```

### 4. Update DB Credentials

Open `DBConnection.java` and modify:

```java
String url = "jdbc:mysql://localhost:3306/employee_db";
String user = "your_username";
String password = "your_password";
```

### 5. Compile and Run

**Using IDE:**

* Open the project and run `Main.java`

**Using CLI:**

```bash
javac -cp .:lib/mysql-connector-java-8.x.x.jar src/*.java
java -cp .:lib/mysql-connector-java-8.x.x.jar src.Main
```

> ⚠️ Make sure the MySQL server is running!

---

## 📁 Project Structure

```bash
Employee-Management-System/
├── src/
│   ├── Main.java
│   ├── Employee.java
│   ├── DBConnection.java
│   ├── EmployeeDAO.java
│   ├── FileHandler.java
│   └── ...
├── resources/
│   └── employees.txt
├── lib/
│   └── mysql-connector-java-8.x.x.jar
├── README.md
└── ...
```

---


## 🤝 Contributing

Contributions are what make the open-source community amazing!
If you'd like to improve this project:

1. 🍴 Fork the repo
2. 🛠 Create your feature branch (`git checkout -b feature/FeatureName`)
3. ✅ Commit your changes (`git commit -m 'Add new feature'`)
4. 🚀 Push to the branch (`git push origin feature/FeatureName`)
5. 📝 Open a Pull Request

---

## 🧑‍💻 Author

**Anshul Yadav**
GitHub: [@Anshul-ydv](https://github.com/Anshul-ydv)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 💡 Fun Fact

> This project stores data in both **MySQL** and **local files** – like a dual-core storage engine! 😄
