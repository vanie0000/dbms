### Data Models and Their Types

A **data model** is an abstract representation that describes how data is organized, stored, and related within a database system. It provides a conceptual framework for understanding the logical arrangement of data and the constraints that govern it. Data models help designers communicate requirements, ensure consistency, and serve as blueprints for database implementation.

* **Hierarchical Model:** Organizes data in a tree structure with one-to-many parent–child relationships. Each child has exactly one parent. It was widely used in early database systems but is inflexible for representing many-to-many relationships.

* **Network Model:** Extends the hierarchical model by allowing a record to have multiple parents. This graph-like structure provides greater flexibility and efficiently represents complex relationships, though it is more difficult to design and maintain.

* **Relational Model:** Represents data as relations (tables) consisting of rows (tuples) and columns (attributes). Based on set theory and first-order predicate logic, it uses SQL for querying and manipulation. Its simplicity, strong theoretical foundation, and support for data integrity have made it the dominant database model.

* **Entity–Relationship (ER) Model:** A high-level conceptual model used during database design. It represents real-world objects as **entities**, their properties as **attributes**, and associations among them as **relationships**. ER diagrams are typically converted into relational schemas during implementation.

* **Object-Oriented Model:** Incorporates object-oriented programming concepts such as objects, classes, inheritance, encapsulation, and methods. It is well suited for applications with complex data types and rich behavior.

* **NoSQL Models:** Designed to handle large-scale, distributed, and semi-structured or unstructured data. Common categories include document stores (for example, MongoDB), key–value stores (for example, Redis), column-family databases, and graph databases. They emphasize scalability, flexibility, and high performance over rigid schemas.

**Placement Tip:** The relational model remains the industry standard for transactional systems, while NoSQL databases are often chosen when horizontal scalability or flexible schemas are primary requirements. Understanding the trade-offs between these models is a frequent interview topic.
