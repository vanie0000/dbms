# 1. Data, Information, Database and File System

## Data

**Definition:**  
Data is a collection of raw facts and figures that can be processed to derive meaning or knowledge. By itself, data has no context or significance.

### Examples
- Orange
- 23
- 100
- Alice

These are simply values until they are interpreted.

---

## Information

**Definition:**  
Information is processed, organized, and meaningful data.

### Examples

**Data**
- Orange
- Color

**Information**
- Orange is a fruit.
- Orange is a color.

Another example:

**Data**
- Alice
- 95

**Information**
- Alice scored 95 marks.

> **Placement Question:** What is the difference between data and information?

**Answer:**

| Data | Information |
|------|-------------|
| Raw facts and figures | Processed data |
| Has no meaning on its own | Has meaningful context |
| Used as input | Produced as output after processing |

---

## Database

### Definition

A **database** is an organized collection of **interrelated data** that is stored electronically and can be efficiently accessed, managed, updated, and retrieved.

In relational databases, data is usually stored in the form of **tables (rows and columns).**

A database can be of any size, ranging from a few records to billions of records.

### Example

**Students Table**

| StudentID | Name | Department |
|-----------|------|------------|
|101|Alice|CSE|
|102|Bob|ECE|

**Courses Table**

| CourseID | StudentID |
|-----------|------------|
|CS101|101|

The two tables are related using **StudentID**.

### Examples of Databases

- College database
- Banking database
- Hospital database
- Airline reservation database
- E-commerce database
- Multimedia database

---

## File System

### Definition

A **file system** is the method used by an operating system to organize, store, and retrieve files on storage devices such as SSDs and hard disks.

Example:

```
Documents/
    Resume.pdf
    Notes.docx

Pictures/

Videos/
```

The operating system knows where each file is stored.

---

## Problems with File Systems

Suppose student records are stored separately by different departments.

```
Library.txt
Hostel.txt
Exam.txt
```

If a student's phone number changes, every file must be updated manually.

If one file is not updated, different files will contain different values.

---

### Disadvantages of File System

### 1. Data Redundancy

The same data is stored multiple times.

Example:
- Student details stored in Library, Hostel, and Exam files.

Problems:
- Wastes storage
- Difficult to maintain

---

### 2. Data Inconsistency

Different copies of the same data may contain different values.

Example:

Library:
```
Phone = 9876543210
```

Hostel:
```
Phone = 9123456780
```

Now the database contains conflicting information.

---

### 3. Poor Memory Utilization

Duplicate copies consume unnecessary storage space.

---

### 4. Difficult Data Sharing

Different applications maintain their own files.

Sharing information becomes difficult.

---

### 5. Security Issues

File systems provide limited security mechanisms.

Sensitive data may be easily modified or accessed.

---

### 6. No Backup and Recovery

Recovering data after accidental deletion or system failure is difficult.

---

### 7. No Concurrency Control

If multiple users modify the same file simultaneously, updates may overwrite one another.

---

## DBMS vs File System

| File System | DBMS |
|-------------|------|
|High redundancy|Reduces redundancy|
|Data inconsistency possible|Maintains consistency|
|Limited security|Strong authentication and authorization|
|No concurrency control|Supports concurrent access|
|Poor backup and recovery|Built-in backup and recovery|
|Limited querying|Supports SQL queries|
|Manual data management|Efficient automated management|

---