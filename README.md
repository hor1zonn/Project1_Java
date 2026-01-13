# First Project Java Spring

A simple Spring Boot web application demonstrating basic web development with Spring Framework, featuring a greeting page with dynamic content.

## 📋 Overview

This is a demo Spring Boot project that showcases:
- Spring Boot MVC web application
- Thymeleaf templating engine
- RESTful endpoints
- Dynamic web content

## 🛠️ Technologies Used

- **Java 21**
- **Spring Boot 4.0.0**
- **Spring Web MVC**
- **Thymeleaf** (template engine)
- **Lombok**
- **Maven** (build tool)

## 📁 Project Structure

```
Project_Vladyslav_Ryzhyk/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── pl/edu/vistula/first_project_java_spring/
│   │   │       ├── ProjectJavaSpringApplication.java
│   │   │       └── controller/
│   │   │           └── HiController.java
│   │   └── resources/
│   │       ├── application.properties
│   │       ├── static/
│   │       │   └── images/
│   │       │       └── helicopter.png
│   │       └── templates/
│   │           └── greeting.html
│   └── test/
├── pom.xml
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Java 21 or higher
- Maven 3.6+ (or use the included Maven Wrapper)

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd Project_Vladyslav_Ryzhyk
   ```

2. Build the project:
   ```bash
   ./mvnw clean install
   ```
   Or on Windows:
   ```bash
   mvnw.cmd clean install
   ```

3. Run the application:
   ```bash
   ./mvnw spring-boot:run
   ```
   Or on Windows:
   ```bash
   mvnw.cmd spring-boot:run
   ```

4. The application will start on `http://localhost:8080`

## 🌐 API Endpoints

### Root Endpoint
- **URL:** `/`
- **Method:** GET
- **Description:** Returns a simple text greeting
- **Response:** `"Hi, its mine spring project."`

### Greeting Page
- **URL:** `/greeting`
- **Method:** GET
- **Description:** Displays a personalized greeting page
- **Query Parameters:**
  - `name` (optional): Name to display in the greeting (default: "World")
- **Example:** `http://localhost:8080/greeting?name=John`

## 📝 Features

- Simple REST endpoint returning plain text
- Dynamic web page using Thymeleaf templates
- Customizable greeting with name parameter
- Static resource serving (images)
- Modern Spring Boot architecture

## 🧪 Testing

Run the test suite:
```bash
./mvnw test
```

Or on Windows:
```bash
mvnw.cmd test
```

## 📦 Build

To create an executable JAR file:
```bash
./mvnw clean package
```

The JAR file will be created in the `target/` directory.

## 👤 Author

**Vladyslav Ryzhyk**

## 📄 License

This project is a demo project for educational purposes.
