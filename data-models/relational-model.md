### Relational Model

The **relational model** represents data in the form of **tables (relations)**. While the ER model provides a conceptual, graphical view of the database, the relational model gives its logical implementation as a collection of interrelated tables.

A relation consists of:

* **Attributes (columns):** Properties of the entity.
* **Tuples (rows/records):** Individual instances of the entity.
* **Domain:** The set of permissible values for an attribute.
* **Degree:** The number of attributes (columns) in a relation.
* **Cardinality:** The number of tuples (rows) in a relation.

For example:

| StudentID | Name | DeptID |
| --------- | ---- | ------ |
| 101       | Asha | CSE    |
| 102       | Ravi | ECE    |

Here, the degree is 3 and the cardinality is 2.

Relations are connected using **foreign keys**, which reference the primary key of another table. For example, a `Department` table with primary key `DeptID` can be referenced by the `Student` table through its `DeptID` column. This establishes relationships and enforces consistency.

The relational model relies on several integrity constraints:

* **Domain integrity:** Attribute values must belong to their specified domains.
* **Entity integrity:** Primary key values must be unique and cannot be NULL.
* **Referential integrity:** A foreign key value must either match an existing primary key value in the referenced table or be NULL (if allowed).

The model follows the **First Normal Form (1NF)** principle that attribute values are **atomic** (indivisible), and every tuple in a relation must be unique.

**Keys:**

* **Super Key:** Any set of attributes that uniquely identifies a tuple.
* **Candidate Key:** A minimal super key.
* **Primary Key:** The candidate key chosen to uniquely identify tuples in the relation.

The relational model’s simplicity, mathematical foundation, and support for powerful query languages such as SQL have made it the most widely used database model in practice.
