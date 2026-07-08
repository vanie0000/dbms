### Entity–Relationship (ER) Model and Its Components

The **Entity–Relationship (ER) model** is a high-level conceptual data model used during database design. It provides a clear, implementation-independent view of the data and its interconnections, making it easier to modify the design as requirements evolve before any database code is written.

Its main components are:

* **Entity:** A distinguishable real-world object or concept about which information is stored, such as a *Student*, *Course*, or *Department*. In ER diagrams, entities are represented by **rectangles**.

* **Attribute:** A property or characteristic that describes an entity or relationship. For example, a Student entity may have attributes such as Roll Number, Name, Age, and Address. Attributes are depicted as **ovals (ellipses)** connected to their entity.

* **Relationship:** An association among two or more entities. For instance, the relationship **STUDIES** may connect the Student and Course entities, indicating which students are enrolled in which courses. Relationships are represented by **diamonds**.

The ER model serves as a bridge between user requirements and the final database schema, helping designers identify data requirements, eliminate ambiguities, and create a robust relational database structure.
