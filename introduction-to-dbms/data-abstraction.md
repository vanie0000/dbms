# 4. Data Abstraction

## Definition

Data abstraction is the process of hiding unnecessary implementation details from users while exposing only the required information.

It allows users to interact with the database without knowing how data is physically stored.

### Real-world Example

While driving a car, you use:
- Steering wheel
- Accelerator
- Brake

You do not need to know how the engine works internally.

Similarly, DBMS hides internal storage details.

---

## Levels of Data Abstraction

### 1. Physical Level (Lowest Level)

Describes **how data is actually stored** inside the database.

Includes:
- Files
- Disk blocks
- Indexes
- B+ Trees
- Storage structures

Handled by database engineers.

---

### 2. Logical Level (Conceptual Level)

Describes **what data is stored** and the relationships among the data.

Example:

Student

- StudentID
- Name
- Department

This level is mainly used by database designers.

---

### 3. View Level (Highest Level)

Shows only the required portion of the database to different users.

Example:

Student View

```
Name
CGPA
Courses
```

Faculty View

```
Attendance
Marks
```

Accounts Department

```
Fee Status
Scholarship
```

Different users access different views of the same database.

---

## Advantages of Data Abstraction

- Simplicity
- Improved security
- Easier maintenance
- Data independence
- Better usability

---
