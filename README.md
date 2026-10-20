# Advanced Java Practical & Lab Repository

A comprehensive collection of core and advanced Java lab projects covering GUI development with MVC, distributed systems with RMI, network socket programming, enterprise web applications with Jakarta Servlets and JSP, database connectivity with JDBC, and the Apache Tomcat 11 application server distribution.

---

## 📂 Repository Structure

```
java-project/
├── 01-calculator-mvc/               # MVC-based Swing Calculator
│   ├── CalculatorModel.java
│   ├── CalculatorView.java
│   ├── CalculatorController.java
│   ├── Main.java
│   └── README.md
│
├── 02-rmi-calculator/               # Remote Method Invocation (RMI)
│   ├── Calculator.java              # Remote Interface
│   ├── CalculatorImplement.java     # Remote Object Implementation
│   ├── Server.java                  # RMI Registry Server
│   ├── Client.java                  # RMI Client
│   └── README.md
│
├── 03-socket-programming/           # TCP Client-Server Networking
│   ├── Server.java                  # ServerSocket on port 5000
│   ├── Client.java                  # Socket client
│   └── README.md
│
├── 04-servlet-demo/                 # Jakarta Servlet 6.1 & Tomcat 11
│   ├── pom.xml
│   ├── src/main/java/com/servlet/   # Servlets, Filters, Listeners
│   └── src/main/webapp/             # index.html
│
├── 05-jsp-servlet-student/          # Jakarta JSP + Servlet Application
│   ├── pom.xml
│   ├── src/main/java/com/servlet/   # HelloServlet
│   └── src/main/webapp/             # student.jsp, result.jsp, web.xml
│
├── 06-student-registration-swing/   # Java Swing Registration Form
│   ├── StudentRegistration.java     # Standalone Swing GUI with validations
│   └── README.md
│
├── 07-student-registration-jdbc/    # Swing GUI + MySQL JDBC Connectivity
│   ├── src/StudentRegistration.java # Form with PreparedStatement CRUD
│   ├── lib/mysql-connector-j-*.jar  # MySQL JDBC Driver
│   ├── schema.sql                   # MySQL Database Schema
│   ├── .vscode/settings.json        # VS Code Java classpath configuration
│   └── README.md
│
├── apache-tomcat-11.0.25/           # Apache Tomcat 11.0.25 Server Distribution
│   ├── bin/                         # Startup and shutdown scripts (catalina.bat, startup.bat, etc.)
│   ├── conf/                        # Server configuration (server.xml, web.xml)
│   ├── lib/                         # Tomcat internal runtime libraries
│   └── webapps/                     # Web application deployment directory
│
└── shopsphere_project/              # ShopSphere E-Commerce Application
    ├── src/com/shopsphere/          # App, Web Server, DAOs, Services, Models
    ├── database/                    # SQL Database Schemas
    ├── data/                        # CSV & Serialized Data Storage
    ├── pom.xml                      # Maven Build Configuration
    └── README.md                    # Project Documentation
```

---

## 🚀 Projects Overview

| # | Project Name | Key Technologies | Description |
|---|---|---|---|
| **01** | [Calculator (MVC)](./01-calculator-mvc/) | Java Swing, MVC Pattern | Desktop calculator separating UI, business logic, and event handling. |
| **02** | [RMI Calculator](./02-rmi-calculator/) | Java RMI, Remote Interface | Distributed system invoking remote arithmetic methods across JVMs. |
| **03** | [Socket Programming](./03-socket-programming/) | `java.net.Socket`, TCP/IP | Client-server communication over stream sockets on port 5000. |
| **04** | [Servlet Demo](./04-servlet-demo/) | Jakarta Servlet 6.1, Tomcat | Comprehensive demo of Servlet Lifecycle, Filters, Listeners, and Session cookies. |
| **05** | [JSP & Servlet App](./05-jsp-servlet-student/) | JSP 3.1, Expression Language | Dynamic web application collecting student info and forwarding to JSP view. |
| **06** | [Student Registration (Swing)](./06-student-registration-swing/) | Java Swing, Form Validation | Desktop GUI form validating user input with `JOptionPane` dialogs. |
| **07** | [Student Registration (JDBC)](./07-student-registration-jdbc/) | JDBC, MySQL, `PreparedStatement` | Desktop database application saving student records into MySQL. |
| **08** | [Apache Tomcat 11.0.25](./apache-tomcat-11.0.25/) | Jakarta EE Servlet Container | Complete pre-configured application server ready to run web applications. |
| **09** | [ShopSphere Project](./shopsphere_project/) | Java SE, JDBC, HTTP Server | Comprehensive multi-tier E-Commerce application with console and embedded web UI. |

---

## 🛠️ Prerequisites

- **Java Development Kit (JDK):** Version 17 or higher
- **Build Tool:** Apache Maven 3.8+ (for Servlet and JSP projects)
- **Servlet Container:** Apache Tomcat 11.0 (included in repository)
- **Database Server:** MySQL Server 8.0+ (for JDBC project)
- **IDE:** Visual Studio Code, IntelliJ IDEA, or Eclipse

---

## ▶️ Quick Execution Guide

### 1. MVC Calculator
```bash
cd 01-calculator-mvc
javac *.java
java Main
```

### 2. RMI Calculator
```bash
cd 02-rmi-calculator
javac *.java
# Terminal 1:
java Server
# Terminal 2:
java Client
```

### 3. Socket Programming
```bash
cd 03-socket-programming
javac *.java
# Terminal 1:
java Server
# Terminal 2:
java Client
```

### 4. Servlet Demo
```bash
cd 04-servlet-demo
mvn clean package
# Copy target/servlet.war into apache-tomcat-11.0.25/webapps/
```

### 5. JSP & Servlet Student App
```bash
cd 05-jsp-servlet-student
mvn clean package
# Copy target/servlet.war into apache-tomcat-11.0.25/webapps/
```

### 6. Swing Student Registration
```bash
cd 06-student-registration-swing
javac StudentRegistration.java
java StudentRegistration
```

### 7. JDBC Student Registration
```bash
cd 07-student-registration-jdbc
# Execute schema.sql in MySQL
javac -cp ".;lib/mysql-connector-j-26.7.0.jar" -d bin src/StudentRegistration.java
java -cp "bin;lib/mysql-connector-j-26.7.0.jar" src.StudentRegistration
```

### 8. Apache Tomcat Server
```bash
cd apache-tomcat-11.0.25/bin
startup.bat
```

---

## 📄 License
This repository is maintained for educational and academic coursework purposes.
