# Spring Boot & Enterprise Java Laboratory Portfolio

This repository hosts practical implementations, software architecture patterns,
and full-stack enterprise systems developed for the Spring Boot and Java Enterprise
curriculum at Mundiapolis University.

---

## Laboratory & Project Overview

| Stage | Module | Core Methodology | Primary Deliverables | Reference |
| :--- | :--- | :--- | :--- | :--- |
| **01. Fundamentals** | **[java-ioc-di-lab](./01-fundamentals/java-ioc-di-lab)** | Inversion of Control (IoC), Dependency Injection (DI), XML vs Component Scan | Loose coupling architecture | [Lab](./01-fundamentals/java-ioc-di-lab/README.md) |
| **02. Persistence** | **[spring-data-jpa-lab](./02-persistence-jpa/spring-data-jpa-lab)** | Spring Data JPA, Hibernate ORM, repositories, auto-DDL schema generation | Entity relational mapping | [Lab](./02-persistence-jpa/spring-data-jpa-lab/README.md) |
| **02. Persistence** | **[spring-jpa-hospital-management](./02-persistence-jpa/spring-jpa-hospital-management)** | Clinical data modeling, complex bidirectional relationships, cascading rules | Healthcare management system | [Lab](./02-persistence-jpa/spring-jpa-hospital-management/README.md) |
| **03. Security** | **[spring-jpa-security-auth-lab](./03-security-auth/spring-jpa-security-auth-lab)** | Spring Security, User-Role RBAC, PasswordEncoder, custom UserDetailsService | Authentication & Authz tier | [Lab](./03-security-auth/spring-jpa-security-auth-lab/README.md) |
| **04. Web MVC** | **[mvc-security-jpa-lab](./04-web-mvc/mvc-security-jpa-lab)** | Server-side MVC architecture, Thymeleaf templates, session security, form validation | Medical consultation web app | [Lab](./04-web-mvc/mvc-security-jpa-lab/README.md) |
| **05. Full-Stack** | **[angular-spring-lab](./05-fullstack-systems/angular-spring-lab)** | Decoupled Spring Boot 3 REST API + Angular 17 SPA, HttpClient, CORS | Product catalog management | [System](./05-fullstack-systems/angular-spring-lab/README.md) |
| **05. Full-Stack** | **[digital-banking-system](./05-fullstack-systems/digital-banking-system)** | Enterprise banking platform, JWT/OAuth2 security, financial ledgers, Angular UI | Full-stack digital bank | [System](./05-fullstack-systems/digital-banking-system/README.md) |

---

## General Running Instructions

### Prerequisites

- **Java Development Kit:** JDK 17 or higher
- **Build Tool:** Apache Maven 3.8+ (or bundled `./mvnw`)
- **Node.js & npm:** Node.js 18+ (for full-stack Angular modules)
- **Database:** In-memory H2 / MySQL 8.0

### Setup and Environment

1. **Clone the repository:**
   ```bash
   git clone git@github.com:ind4x/spring-boot-portfolio.git
   cd spring-boot-portfolio
   ```

### Executing Backend Modules
Navigate into any lab subdirectory and execute via the embedded Maven wrapper:

```bash
cd 02-persistence-jpa/spring-data-jpa-lab
./mvnw spring-boot:run
```

Access the H2 database console (when enabled) at `http://localhost:8080/h2-console`.

### Executing Full-Stack Modules
For modules with an Angular frontend (e.g., `05-fullstack-systems/digital-banking-system`):

1. **Launch Spring Boot Backend:**
   ```bash
   cd 05-fullstack-systems/digital-banking-system/backend
   ./mvnw spring-boot:run
   ```
2. **Launch Angular Frontend:**
   ```bash
   cd 05-fullstack-systems/digital-banking-system/frontend
   npm install
   npm start
   ```
   Open `http://localhost:4200` in your web browser.

---

## Technology Stack

- **Backend:** Java 17+, Spring Boot 3.x, Spring Data JPA, Spring Security, Hibernate
- **Frontend:** Angular 17, TypeScript, HTML5/CSS3, Bootstrap
- **Persistence & DB:** H2 In-Memory Database, MySQL, PostgreSQL
- **Build & Dependency Management:** Maven (`pom.xml`)

---

## Author

- **Author:** Youssef Fellah ([ind4x_](https://github.com/ind4x))
- **Institution:** Mundiapolis University, Engineering Cycle
