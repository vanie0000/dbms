### ER Diagrams

An **Entity–Relationship (ER) diagram** is a graphical representation of the overall logical structure of a database. It provides a simple and clear way to visualize entities, their attributes, and the relationships among them, making it one of the most widely used tools in database design.

* **Strong Entity Set:** Has its own primary key and exists independently. Example: **Student** with key `RollNo`.
* **Weak Entity Set:** Does not have a complete key of its own and depends on a strong entity for identification. It is shown by a **double rectangle**. Example: **Dependent** of an Employee, identified by `(EmpID, DependentName)`.
* **Identifying (Strong–Weak) Relationship:** Connects a weak entity to its owner entity and is drawn with a **double diamond**. Example: Employee–Has–Dependent.

**Types of Attributes**

* **Single-valued:** One value per entity (e.g., DateOfBirth).
* **Composite:** Can be decomposed into subparts (e.g., Address → Street, City, ZIP).
* **Multivalued:** Multiple values are allowed (e.g., PhoneNumbers); represented by a **double ellipse**.
* **Derived:** Computed from other attributes (e.g., Age derived from DateOfBirth); represented by a **dashed ellipse**.
* **Null/Optional:** May not have a value for some entities (e.g., MiddleName).
* **Complex:** A combination of composite and multivalued attributes (e.g., multiple Addresses, each with Street, City, and ZIP).

**Participation Constraints**

* **Total Participation:** Every entity must participate in the relationship; shown by a **double line**. Example: Every Enrollment must involve a Student.
* **Partial Participation:** Participation is optional; shown by a **single line**.

**Recursive (Unary) Relationship:** An entity relates to itself. Example: An Employee **manages** another Employee.

**Cardinality Ratios**

* **One-to-One (1:1):** One Person has one Passport.
* **One-to-Many (1:N):** One Department employs many Employees.
* **Many-to-One (N:1):** Many Employees belong to one Department.
* **Many-to-Many (M:N):** Students enroll in many Courses, and Courses have many Students.

ER diagrams are invaluable because they allow designers to refine the schema and capture business rules before implementing the database, reducing costly changes later in development.

Here are a few classic ER-diagram examples:

* **Student–Course Enrollment:** `Student(RollNo, Name)` — **ENROLLS** — `Course(CourseID, Title)` with cardinality **M:N**.
* **Department–Employee:** `Department(DeptID, DeptName)` — **EMPLOYS** — `Employee(EmpID, Name)` with cardinality **1:N** and total participation of Employee.
* **Employee–Dependent (Weak Entity):** `Employee(EmpID, Name)` — **HAS** — `Dependent(DependentName, DOB)` where `Dependent` is a weak entity identified by `(EmpID, DependentName)`.
* **Employee Supervises Employee:** A recursive relationship `Employee` — **SUPERVISES** — `Employee`, typically with cardinality **1:N** (one manager supervises many employees).

These examples cover the most important ER concepts: many-to-many relationships, participation constraints, weak entities, and recursive relationships. Sketching them with the standard ER symbols (rectangles for entities, ovals for attributes, diamonds for relationships, and the appropriate cardinality labels) is excellent practice for exams and interviews.