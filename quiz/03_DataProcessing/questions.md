# quiz question and answers

- [What is a Database?](#what-is-a-database)
- [What is Data Base Management System?](#what-is-data-base-management-system)
- [What is a Relational Database (E.F. Codd's relational model)?](#what-is-a-relational-database-ef-codds-relational-model)
- [What is a Relational Database Management System (RDBMS)?](#what-is-a-relational-database-management-system-rdbms)
- [What is a table(relation)?](#what-is-a-tablerelation)
- [What is a Record or a Row (Tuple)?](#what-is-a-record-or-a-row-tuple)
- [What is an attribute or a column?](#what-is-an-attribute-or-a-column)
- [What is a field?](#what-is-a-field)
- [What are SQL Constraints](#what-are-sql-constraints)
- [What are Primary Keys and Foreign Keys?](#what-are-primary-keys-and-foreign-keys)
- [What are Simple and Composite Keys?](#what-are-simple-and-composite-keys)
- [What are Natural Primary Key and Surrogate Primary Key?](#what-are-natural-primary-key-and-surrogate-primary-key)
- [What is Database Normalization?](#what-is-database-normalization)
- [What is First Normal Form?](#what-is-first-normal-form)
- [What is Second Normal Form?](#what-is-second-normal-form)
- [What is Third Normal Form?](#what-is-third-normal-form)
- [What are Anomalies in Data Bases?](#what-are-anomalies-in-data-bases)
- [How to develop a model of the real world?](#how-to-develop-a-model-of-the-real-world)
- [How to design a table?](#how-to-design-a-table)
- [What is ACID?](#what-is-acid)
- [What is SQL?](#what-is-sql)
- [What are data definition queries?](#what-are-data-definition-queries)
- [How to create a table with relations using CREATE TABLE syntax and attribute data types?](#how-to-create-a-table-with-relations-using-create-table-syntax-and-attribute-data-types)
- [How to establish table indexes?](#how-to-establish-table-indexes)
- [What are One-to-many, One-to-one and Many-to-many relationships?](#what-are-one-to-many-one-to-one-and-many-to-many-relationships)
- [How to use Cascading changes and Cascading Deletion?](#how-to-use-cascading-changes-and-cascading-deletion)
- [What is Database Denormalization?](#what-is-database-denormalization)
- [What are transactions and how do they work?](#what-are-transactions-and-how-do-they-work)
- [What are triggers and how do they work?](#what-are-triggers-and-how-do-they-work)
- [What database object naming considerations do you know?](#what-database-object-naming-considerations-do-you-know)

### What is a Database?

Definitions:

- A database is **an organized collection of data**, generally stored and accessed electronically from a computer system.
- A database is **a collection of information** that is organized so that it can be easily accessed, managed and updated.
- A database is **a data structure** that stores organized information.

### What is Data Base Management System?

`Data Base Management System` is **a software package** designed to
**define, manipulate, retrieve and manage data** in a database. A `DBMS`
generally manipulates the data itself, the data format, field names,
record structure and file structure. It also **defines rules** to validate
and manipulate this data.

- **Functions of DBMS:**
  - Provides data Independence
  - Concurrency Control
  - Provides Recovery services
  - Provides Utility services
  - Provides a clear and logical view of the process that manipulates data.
- **Advantages of DBMS**
  - Segregation of application program.
  - Minimal data duplicity.
  - Easy retrieval of data.
  - Reduced development time and maintenance need
- **Disadvantages of DBMS**
  - Complexity
  - Costly
  - Large

### What is a Relational Database (E.F. Codd's relational model)?

`A relational database (RDB)` is a **collective set of multiple data sets** organized by **tables**, **records** and **columns**. `RDBs` establish a well-defined relationship between database tables. Tables communicate and share information, which facilitates data searchability, organization and reporting. `RDBs` use `Structured Query Language (SQL)`
`RDB` is derived from the mathematical function concept of **mapping data sets.**

Traditional `RDBs` store data in highly structured tabular form, with multiple **rows and columns**. While these data stores are highly flexible, easy to maintain, and effective for data stored on a single server, _they do not scale very well in a distributed system_ **compared** to `NoSQL` database alternatives. `NoSQL` databases do not use the standard tabular relationships the relational databases employ. Instead, `NoSQL` databases allow for the querying and storage of data by a variety of other means, depending on thespecific software.

- Data models used in `NoSQL` databases are:
  - document model,
  - graph model,
  - key-value model

### What is a Relational Database Management System (RDBMS)?

Examples of popular `RDBMS` systems include:

- Microsoft SQL Server
- MySQL
- Oracle Database
- PostgreSQL
- SQLite

A Relational Database Management System (RDBMS) is a **type of database management system** that **organizes data into tables**, where **data elements are related to each other** based on predefined relationships. The relationships are established using **keys**, allowing the `RDBMS` to manage and maintain the integrity of the data.

> **Tabular Structure:**
>
> Data is organized into tables, where each table consists of rows and columns. Each row represents a record, and each column represents an attribute or field.

> **Data Integrity:**
>
> RDBMS enforces data integrity by supporting constraints such as primary keys, foreign keys, unique constraints, and check constraints. These constraints ensure the accuracy and consistency of the stored data.

> **ACID Properties:**
>
> RDBMS systems adhere to the ACID properties (Atomicity, Consistency, Isolation, Durability), ensuring transactions are processed reliably and securely.

> **SQL (Structured Query Language):**
>
> `RDBMS` systems use SQL for data definition, manipulation, and control. SQL provides a standardized language for interacting with relational databases.

> **Relational Algebra:**
>
> `RDBMS` systems operate based on relational algebra principles, allowing users to perform operations such as selection, projection, union, intersection, and join on tables.

> **Normalization:**
>
> `RDBMS` supports normalization techniques to eliminate data redundancy and improve data integrity. Normalization involves organizing tables to reduce data duplication and improve efficiency.

> **Concurrency Control:**
>
> `RDBMS` systems manage concurrent access to the database by multiple users or applications. Techniques such as locking and transaction isolation levels are employed to maintain consistency in a multi-user environment.

> **Data Independence:**
>
> `RDBMS` provides a level of data independence, separating the physical storage details from the logical data model. This allows changes to the physical storage without affecting the application or higher-level logical model.

> **Scalability:**
>
> `RDBMS` systems are designed to scale horizontally or vertically to accommodate growing data and user demands. This scalability ensures that the system can handle increased workloads.

### What is a table(relation)?

**Tables** – In the Relational model the relations are saved in the table format. It is stored along with its entities. A table has two properties rows and columns. Rows represent records and columns represent attributes.

**Relation Schema** - A relation schema represents the name of the relation with its attributes.

**Relation instance** – Relation instance is a finite set of tuples in the RDBMS system. Relation instances never have duplicate tuples

### What is a Record or a Row (Tuple)?

**Tuple** – It is a single row of a table, which contains a single record
**Cardinality** - Total number of rows present in the Table.

### What is an attribute or a column?

**Attribute** - Each column in a Table. Attributes are the properties which define a relation.
**Attribute domain** – Every attribute has some pre-defined value and scope which is known as attribute domain

**Degree** - The total number of attributes which in the relation is called the degree of the relation.

### What is a field?

filed is a _cell_ - holding value, a single piece of information of row

### What are SQL Constraints

`Constraints` are used to **specify rules** for the data in a table.
`Constraints` are used to **limit the type** of data that can go into a table

### What are Primary Keys and Foreign Keys?

- `Foreign Key` **references** `Primary Key`

**Primary Key**

- Helps you to uniquely identify a record in the table.
- Primary Key never accept null values.
- Primary key is a clustered index and data in the DBMS table are physically organized in the sequence of the clustered index.
- You can have the single Primary key in a table.

---

**Foreign Key**

- It is a field in the table that is the primary key of another table.
- A foreign key may accept multiple null values
- A foreign key cannot automatically create an index, clustered or non-clustered. However, you can manually create an index on the foreign key
- You can have multiple foreign keys in a table

### What are Simple and Composite Keys?

- **Simple key** consists of single column that uniquely identifies rows in a table.
- **Composite key** is a combination of **two or more columns** that uniquely identify rows in a table. The combination of columns guarantees uniqueness, though individually uniqueness is not guaranteed.

### What are Natural Primary Key and Surrogate Primary Key?

**A natural key** is primary key that consist of table information fields (that is, fields containing useful information about the described objects). Such primary key is called .

In practice, the use of **natural keys** runs into certain **difficulties**:

- low efficiency (size, need to duplicate in case of migration);
- cascading changes;
- inconsistency with reality (the value of the field selected as the primary key can be specified later)

---

**Surrogate keys** is an artificial key which aims to **uniquely identify** each record is called a surrogate key. This kind of partial key in dbms is unique because it is created when you don't have any natural primary key. _They do not lend any meaning to the data in the table._ Surrogate key is usually an **integer**. A surrogate key is a value generated **right before** the record is inserted into a table.

---

> COMPARASION:
>
> **Problems with Natural Key:**
>
> - Big size.
> - Requires for cascading changes.
> - Impossible to insert data in case of information absence
>
> **Advantages of Surrogate Key:**
>
> - Small size.
> - Not requires for cascading changes.
> - You can insert data even if some information is missing

### What is Database Normalization?

`NORMALIZATION` is a database design technique that **reduces data redundancy** and eliminates undesirable characteristics like Insertion, Update and Deletion **Anomalies**.

`Normalization` rules divides larger tables into smaller tables and links them using **relationships**. The purpose of `Normalization` in SQL is to **eliminate redundant (repetitive)** data and ensure data is **stored logically**.

**Normalization requirements**

- Relationship `primary keys` should be **minimal**
- The database model should **minimize or eliminate data redundancy** whenever possible
- The database model should provide the **required performance** of operations
- The database model should **minimize data inconsistency** in all data operations(The relationships must be established EXPLICITLY!)
- The database model must be **adaptable** if changes are required. This is achieved by:
  - Mnemonic names.
  - Comments.
  - Documentation.
  - Schemes in generally accepted notation.
  - No stupid restrictions
- Always the database **must contain an actual data set** (not old or unactuall)

### What is First Normal Form?

- each table cell should contain **a single value** ( NOT AN ARRAY etc)
  so ex: multiple rows for customer with rented movies

- each record to be **unique**

### What is Second Normal Form?

- be in `First Normal Form`
- have a `primary key` or `composite key` (whole)

usually requires **spliting tables** => use of `foreign key` (ex: table of _rented movies_ and table of _customers_)

helps with **referental integrity** ( when inserting into `rented movies` and using customer_id that doesnt exsits -> ERROR)

### What is Third Normal Form?

- be in `First Normal Form`
- has no **transitive functional dependencies**

usually requires **spliting tables** ex: column _salutation_ "Mr"/"Ms" => when changing way of salutation no need to update every row-> table of salutations (ex. salutation_id)

### What are Anomalies in Data Bases?

`Anomaly` is contradiction between the domain model and the data model supported by the means of a specific `DBMS`.
This problems can occur in poorly planned, unnormalized databases where all data is stored in one table (a flat-file database)

Types of anomalies:

- **Insert** (attributes cannot be inserted into the database without
  the presence of other attributes)
- **Update** (when one or more instances of duplicated data is updated, but not all.)
- **Delete** (attributes are lost because of the deletion of other
  attributes)

### How to develop a model of the real world?

- Identify Entities:
- Define Relationships:
- Identify Attributes:
- Normalize Data:

### How to design a table?

- Define Table Name:
- Identify Primary Key:
- Determine Data Types:
- Handle NULL Values:
- Define Constraints:
- Normalize the Table:
- Establish Relationships:
- Consider Indexing:
- Review and Iterate:
- Document the Table:

### What is ACID?

`ACID` is a set of properties of DB operations intended to **guarantee validity** even in the event of **errors**, **power failures**, etc.

In the context of DBs, **a sequence of database operations** that satisfies the `ACID` properties (which can be perceived as a single logical operation on the data) is called a **transaction**

### What is SQL?

### What are data definition queries?

**Data Definition Queries (DDQ)** are **SQL statements** used to define, modify, or delete database objects such as tables, indexes, views, constraints, and other schema-level elements. These **queries** are part of the **Data Definition Language (DDL)** in `SQL`, which is responsible for defining and managing the structure of the database.

### How to create a table with relations using CREATE TABLE syntax and attribute data types?

```
-- Creating the Departments table
CREATE TABLE Departments (
    DepartmentID INT PRIMARY KEY,
    DepartmentName VARCHAR(100) NOT NULL
    -- Other columns specific to the Departments table
);

-- Creating the Employees table with a foreign key relationship to Departments
CREATE TABLE Employees (
    EmployeeID INT PRIMARY KEY,
    FirstName VARCHAR(50) NOT NULL,
    LastName VARCHAR(50) NOT NULL,
    DepartmentID INT,

    -- Defining a foreign key constraint referencing Departments table
    FOREIGN KEY (DepartmentID) REFERENCES Departments(DepartmentID)
);
```

### How to establish table indexes?

The Employee table has a **primary key** constraint on EmployeeID and a **single column index** on DepartmentID.

```
-- Creating a table with a primary key and a single column index
CREATE TABLE Employee (
    EmployeeID INT PRIMARY KEY,
    FirstName VARCHAR(50),
    LastName VARCHAR(50),
    DepartmentID INT,
    -- Other columns

    -- Creating a single column index on DepartmentID
    INDEX idx_DepartmentID (DepartmentID)
);
```

The Product table has a **primary key constraint** on ProductID and a **composite index** on CategoryID and VendorID.

```
-- Creating a table with a composite (multi-column) index
CREATE TABLE Product (
    ProductID INT PRIMARY KEY,
    CategoryID INT,
    VendorID INT,
    ProductName VARCHAR(100),
    -- Other columns

    -- Creating a composite index on CategoryID and VendorID
    INDEX idx_Category_Vendor (CategoryID, VendorID)
);
```

The Customer table has a **primary key constraint** on CustomerID and a **unique index** on Email.

```
-- Creating a table with a unique index
CREATE TABLE Customer (
    CustomerID INT PRIMARY KEY,
    Email VARCHAR(100) UNIQUE,
    FirstName VARCHAR(50),
    LastName VARCHAR(50),
    -- Other columns
);
```

The OrderDetails table has a **primary key constraint** on OrderDetailID with **a clustered index** (SQL Server specific) and a non-clustered index on OrderID.

```
-- Creating a table with a clustered index (SQL Server specific)
CREATE TABLE OrderDetails (
    OrderDetailID INT PRIMARY KEY CLUSTERED,
    OrderID INT,
    ProductID INT,
    Quantity INT,
    -- Other columns

    -- Creating a non-clustered index on OrderID
    INDEX idx_OrderID NONCLUSTERED (OrderID)
);
```

### What are One-to-many, One-to-one and Many-to-many relationships?

### How to use Cascading changes and Cascading Deleteion?

`Cascading changes` and `cascading deletions` refer to the automatic propagation of changes or deletions from one table to another when a related record is updated or deleted. This behavior is often defined through **foreign key** relationships between tables.

- **Cascading Changes:** are used when you want changes in the primary key of one table to automatically reflect in the foreign key references in other tables.

  **Creating a Foreign Key with Cascading Changes:**

  ```
  ALTER TABLE ChildTable
  ADD CONSTRAINT FK_ChildTable_ParentTable
  FOREIGN KEY (ParentID) REFERENCES ParentTable(ID)
  ON UPDATE CASCADE;
  ```

  In this example, changes to the ID column in the ParentTable will automatically cascade to the ParentID column in the ChildTable.

---

- **Cascading deletions** are used when you want the deletion of a record in the primary table to automatically result in the deletion of related records in the referencing table.

  **Creating a Foreign Key with Cascading Deletions:**

  ```
      ALTER TABLE ChildTable
      ADD CONSTRAINT FK_ChildTable_ParentTable
      FOREIGN KEY (ParentID) REFERENCES ParentTable(ID)
      ON DELETE CASCADE;
  ```

  In this example, deleting a record in the ParentTable with a matching ID will automatically delete all related records in the ChildTable with the corresponding ParentID.

### Example:

Let's consider two tables: Customers and Orders, where Orders has a foreign key reference to Customers.

```
CREATE TABLE Customers (
    CustomerID INT PRIMARY KEY,
    CustomerName VARCHAR(255)
);

CREATE TABLE Orders (
    OrderID INT PRIMARY KEY,
    OrderNumber VARCHAR(255),
    CustomerID INT,
    FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID) ON DELETE CASCADE
);
```

With the ON `DELETE CASCADE` in the foreign key constraint, if you delete a customer from the Customers table, all corresponding orders in the Orders table with the matching CustomerID will be automatically deleted.

### What is Database Denormalization?

- the process of making relationships to a state that **violates certain** normal forms
  reason: cache tables make some operations performed much faster than on a set of source tables

### What are transactions and how do they work?

**a sequence of database operations** that satisfies the `ACID` properties (which can be perceived as a single logical operation on the data)

`ACID` is an acronym that stands for

- **Atomicity**
  - Transferring founds from one account to another: 2 update in the table of accounts and 1 insert in the table of transfers. In this case, operations constitute a unit of work: either all or nothing required
- **Consistency**
  - Changes do not contradict database restrictions: PK, FK, check
- **Isolation**
  - The result should be visible only after performing all operations
- **Durability**
  - After the operation is completed, the data is available and lost

### What are triggers and how do they work?

Triggers is a special type of stored procedure that automatically takes effect when a **Data Manipulation Language (DML) event** takes place that affects the table.

Triggers in a database are special types of stored procedures that automatically execute (or "trigger") in response to specific events or changes in the database. These events include INSERT, UPDATE, DELETE operations on specific tables or views. Triggers are often used for enforcing business rules, maintaining data integrity, or automating complex database operations.

**Key Concepts:**

> **Event:**
>
> An action that occurs in the database, such as an `INSERT`, `UPDATE`, or `DELETE` operation.

> **Trigger Type:**
>
> There are three main types of triggers: `BEFORE`, `AFTER`, and `INSTEAD OF`. `BEFORE` triggers execute before the event, `AFTER` triggers execute after the event, and `INSTEAD OF` triggers replace the original event.

> **Timing:**
>
> - `BEFORE` triggers can be used to validate or modify data before it is written to the database.
> - `AFTER` triggers are often used for actions that need to occur after the data is written to the database.

> **Use Cases:**
>
> - Enforcing business rules.
> - Automatically updating timestamp fields.
> - Logging changes to the database.

**Example:**

```
CREATE TRIGGER before_insert_employee
BEFORE INSERT ON Employees
FOR EACH ROW
BEGIN
    -- Trigger logic here
    -- You can access NEW.column_name to refer to the new value being inserted
    -- For example, : NEW.EmployeeID, NEW.FirstName, NEW.LastName
END;
```

### What database object naming considerations do you know?

### T-SQL

- Data Manipulation Language (DML)

  ```
  INSERT INTO (Table) VALUES (list of values)
  ```

- Data Query Language (DQL)

  ```
  SELECT (list of columns) FROM (table)
  ```

- Data Definition Language (DDL)

  ```
  CREATE (object) (name)
  ```

- Transaction Control Language (TCL)

  ```
  COMMINT TRANSACTION (name)
  ```

- Data Control Language (TCL)

  ```
  GRANT CONTROL (object) TO (user)
  ```
