# Software Engineering at Wells Fargo

This repository is a backend system for managing financial advisors and their clients’ portfolios. It is built with **Spring Boot** and uses the **Java Persistence API (JPA)** to manage data persistence in a relational database. The system enables financial advisors to create, update, and remove clients, as well as manage portfolios and securities.  

---

## 📌 Features  
- Manage multiple **financial advisors** and their **clients**  
- Each client has a **portfolio** that may contain multiple **securities**  
- Financial advisors can:  
  - Add, update, and remove clients  
  - Add, update, and remove securities in client portfolios  
- Securities track the following attributes:  
  - Name  
  - Category  
  - Purchase date  
  - Purchase price  
  - Quantity  

---

## 🗄️ Data Model (ERD)  

The system is modeled using an **Entity Relationship Diagram (ERD)**.  

**Entities & Relationships**:  
- **FinancialAdvisor** → one-to-many with **Client**  
- **Client** → one-to-one with **Portfolio**  
- **Portfolio** → one-to-many with **Security**  
- **Security** → belongs to a **Portfolio**  

---

## ⚙️ Technologies Used  
- **Java 17+**  
- **Spring Boot** (REST API + JPA integration)  
- **JPA / Hibernate** (ORM for relational database persistence)  
- **H2 / PostgreSQL** (configurable relational database)  
- **Maven** (dependency management and build)  
