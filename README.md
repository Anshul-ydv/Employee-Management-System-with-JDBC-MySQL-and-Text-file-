# Employee Management System 📋

A simple and functional **Employee Management System** built using **Java**, with **JDBC** for database connectivity and **MySQL** as the backend. The system also includes support for reading and writing employee data via **text files**.

---

## 💡 Features

- Add, update, delete, and search employee records
- Store employee data in both MySQL database and text files
- Clean and modular Java code using OOP principles
- Simple console-based interface for ease of use
- JDBC for secure and efficient database connectivity

---

## 🛠️ Tech Stack

| Technology | Description |
|------------|-------------|
| Java       | Core application logic and console interface |
| JDBC       | Database connectivity layer |
| MySQL      | Persistent storage for employee data |
| Text Files | Backup and local storage for records |

---

## 🚀 Getting Started

### Prerequisites

- Java JDK (version 8 or later)
- MySQL Server
- Any IDE (IntelliJ, Eclipse, VS Code) or command line
- MySQL JDBC Driver (e.g., `mysql-connector-java-8.x.x.jar`)

---

### 🔧 Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/Employee-Management-System.git
   cd Employee-Management-System
````

2. **Import the project** into your Java IDE or compile using CLI.

3. **Configure MySQL**

   * Create a database in MySQL:

     ```sql
     CREATE DATABASE employee_db;
     ```
   * Use the provided `.sql` file (if available) to create the `employee` table, or manually run:

     ```sql
     CREATE TABLE employee (
         id INT PRIMARY KEY,
         name VARCHAR(100),
         age INT,
         department VARCHAR(100),
         salary DOUBLE
     );
     ```

4. **Update DB credentials**

   * Modify the `DBConnection.java` or equivalent file with your MySQL username, password, and DB name.

5. **Run the application**

   * Run the `Main.java` or `EmployeeManagementSystem.java` file.

---

## 📂 Project Structure

```bash
Employee-Management-System/
│
├── src/
│   ├── Main.java
│   ├── DBConnection.java
│   ├── Employee.java
│   ├── EmployeeDAO.java
│   ├── FileHandler.java
│   └── ...
├── resources/
│   └── employees.txt  # text file for storing records
├── lib/
│   └── mysql-connector-java-8.x.x.jar
├── README.md
└── ...
```

---

## 📌 Notes

* Ensure MySQL server is running before starting the app.
* Records are backed up to `employees.txt` for redundancy.
* JDBC driver `.jar` must be added to your classpath when compiling/running.

---

## 🧑‍💻 Author

**Anshul Yadav**
[GitHub](https://github.com/Anshul-ydv)
[LinkedIn](https://linkedin.com/in/anshulydv)

---

## 📃 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🤝 Contributions

Feel free to fork the repo and submit pull requests. Issues and suggestions are welcome!
