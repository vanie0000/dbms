# 5. Three-Tier Architecture

Modern DBMS-based applications are divided into three logically separate layers.

```
+---------------------------+
|   Presentation Layer      |
+---------------------------+
            |
+---------------------------+
|   Application Layer       |
+---------------------------+
            |
+---------------------------+
|      Data Layer           |
+---------------------------+
```

---

## 1. Presentation Layer (Client Layer)

Responsible for user interaction.

Examples:
- Web browser
- Desktop application
- Mobile application

Responsibilities:
- Display data
- Accept user input
- Send requests to the application layer

---

## 2. Application Layer (Business Logic Layer)

Contains the business rules of the application.

Responsibilities:
- Authentication
- Validation
- Business logic
- Processing user requests
- Communicating with the database

Examples:
- Login verification
- Payment processing
- Discount calculation
- REST APIs

---

## 3. Data Layer (Database Layer)

Responsible for storing and managing data.

Responsibilities:
- SQL query execution
- Data storage
- Data retrieval
- Transaction management
- Backup and recovery
- Index management

---

## Advantages of Three-Tier Architecture

- Better scalability
- Improved modularity
- Easier maintenance
- Better security
- Reusable business logic
- Improved performance through separate servers

---

## Disadvantages of Three-Tier Architecture

- Increased complexity
- Longer development time
- Higher infrastructure cost
- Potential network latency
- Additional resource overhead
- Possible bottlenecks in the application layer

---

# Placement Revision (Most Frequently Asked)

## ⭐⭐⭐ Very Important

- Difference between Data and Information
- Difference between File System and DBMS
- Advantages of DBMS over File System
- Data Redundancy vs Data Inconsistency
- Three Levels of Data Abstraction
- Three-Tier Architecture
- Applications of DBMS

---

## ⭐⭐ Important

- Types of Databases
- Advantages and Disadvantages of DBMS
- Need for DBMS

---

## ⭐ Common Interview Questions

1. What is DBMS?
2. Why is DBMS preferred over a file system?
3. Explain data redundancy and data inconsistency with examples.
4. What are the advantages of DBMS?
5. Explain the three levels of data abstraction.
6. Explain three-tier architecture with a real-world example.
7. What are the different types of databases?
8. Difference between relational databases and NoSQL databases.
9. What are the functions of a DBMS?
10. What are the real-world applications of DBMS?