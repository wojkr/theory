# Index:

[Primary Key](#primary-key)
[Foreign Key](#foreign-key)
[ACID](#acid-principles-of-transactions---brief-description)
[Normalization](#normalization)
[Other Naming](#other-naming)

### Primary ey

- The primary key is used to identify each record in the table.
  correct

- The primary key cannot be `NULL`.
  correct

- A table **CANNOT** have more than one primary key.

- The primary key, by default, creates clustered index.
  correct

- You **CANNOT** change the value of the primary key, but you can't delete it.
  > It is not possible to edit primary key of the record because primary is identifier of record which identifies record based on that value. If you change primary key it will be considered as new record.

[Back To Index](#index)

### Foreign key

- The foreign key is a field in the table that is the primary key of another table.

- The foreign key may take multiple `NULL` values.

- The foreign key, by default, **DOES NOT** create clustered index.

- Index for foreign key can be created manually.

- There might be more than one foreign key in the table.

[Back To Index](#index)

### ACID principles of transactions - brief description

- Atomicity - The transaction is either completed or entirely undone. There can be no partial transaction.

- Isolation: Each transaction must execute independent of any other transaction.

- Consistency: The transaction must transform the database from one consistent state to another.

- Durability: Completed transactions are permanent.

[Back To Index](#index)

### Normalization

**The normalization**

- is the process of organizing the data in the database.

- is used to minimize the redundancy from a relation or set of relations.

- The normalization divides the larger table into smaller and links them using relationships.

- The normalization is used to reduce redundancy from the database table.

**Normal Forms**

1. An entity is in the first normal form if it contains no repeating groups.

2. An entity is in the second normal form if it is in the first normal form and all of its attributes depend on the whole (primary) key.

3. An entity is in the third normal form if it is in the second normal form and all of its attributes are not transitively dependent on the primary key.

[Back To Index](#index)

### Other naming

**Table**

> Relation - Table - File

**Column**

> Attribute - Column - Field

**Row**

> Tuple - Row - Record

[Back To Index](#index)
