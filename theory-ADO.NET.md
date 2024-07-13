# ActiveX Data Objects for .NET

[DbDataReader](#dbdatareader)
[DbDataCommand](#dbdatacommand)
[DbDataConnection](#dbdataconnection)
[DbDataAdapter](#dbdataadapter)

[ExecuteNonQuery](#executenonquery)
[ExecuteReader](#executereader)
[ExecuteScalar](#executescalar)

# Summary of ADO.NET

ADO.NET (ActiveX Data Objects for .NET) is a set of computer software components that programmers can use to access data and data services. It is part of the .NET Framework and provides a bridge between the front end (user interface) and the back end (database). ADO.NET is designed to work with relational databases, XML, and other data sources, allowing for efficient data manipulation and management.

### Classes that make up a data provider include:

- `DbCommand`
- `DbDataReader`
- `DbConnection`
- `DbDataAdapter`

[Back To Index](#activex-data-objects-for-net)

## Overview

ADO.NET is designed to provide consistent access to data sources such as SQL Server and XML, and it includes a variety of data access methods and objects. It operates in both connected and disconnected modes, offering flexibility and efficiency in handling data. ADO.NET uses a `DataSet` object for disconnected data manipulation, and it supports a rich set of data access operations, such as querying, updating, and managing data.

[Back To Index](#activex-data-objects-for-net)

## Three Most Important Methods/Objects/Interfaces

### 1. SqlConnection

**Description**: Represents a connection to a SQL Server database. It is used to establish a connection with the database and manage the connection's lifecycle.

**Key Methods**:

- `Open()`: Opens the database connection.
- `Close()`: Closes the database connection.
- `BeginTransaction()`: Starts a database transaction.

**Example**:

```csharp
using (SqlConnection connection = new SqlConnection(connectionString))
{
    connection.Open();
    // Perform database operations
    connection.Close();
}
```

[Back To Index](#activex-data-objects-for-net)

### 2. SqlCommand

**Description**:

Represents a SQL statement or stored procedure to execute against a SQL Server database. It is used to execute queries and commands, such as `SELECT`, `INSERT`, `UPDATE`, and `DELETE`.

**Key Methods**:

- `ExecuteReader()` method of the `DbCommand` class is the best suited when you execute a `SELECT` query and return a reader object that wraps a readonly, forward-only cursor. Executes the command and returns a `SqlDataReader` for reading the results.
- `ExecuteNonQuery()` method of the `DbCommand` class is the best suited when you execute non-SELECT commands, such as SQL commands that **insert, delete, update** records or execute datadefinition commands that `create`, `alter`, or `delete` database objects (such as tables, indexes, constraints, and so on). Executes the command and returns the number of rows affected.
- `ExecuteScalar()` method of the `DbCommand` class is the best suited when you have aggregate SQL functions in a `SELECT` statement. Executes the command and returns a single value.

[Back To Index](#activex-data-objects-for-net)

**Example**:

```csharp
using (SqlCommand command = new SqlCommand(queryString, connection))
{
    SqlDataReader reader = command.ExecuteReader();
    while (reader.Read())
    {
        Console.WriteLine(reader[0].ToString());
    }
}
```

[Back To Index](#activex-data-objects-for-net)

### 3. DataSet

**Description**:

The `DataSet` represents an in-memory cache of data. It is a disconnected, in-memory representation of data that can hold multiple tables and relationships between them. It is ideal for working with data without needing a constant connection to the data source.

**Key Methods**:

- **`ReadXml()`**: Reads XML schema and data into the `DataSet`.
- **`WriteXml()`**: Writes the current `DataSet` as an XML document.
- **`Merge()`**: Merges the specified `DataSet` with the current `DataSet`.

**Example**:

```csharp
DataSet dataSet = new DataSet();
dataSet.ReadXml("data.xml");

foreach (DataTable table in dataSet.Tables)
{
    foreach (DataRow row in table.Rows)
    {
        Console.WriteLine(row["ColumnName"]);
    }
}
```

### DbDataReader

**DbDataReader** Provides read-only data access in the forward direction with a server-side cursor.

[Back To Index](#activex-data-objects-for-net)

<br>

### DbDataCommand

**DbDataCommand** Represents a SQL query or stored procedure and also provide access to the read object provider-specific data.

[Back To Index](#activex-data-objects-for-net)

<br>

### DbDataConnection

**DbDataConnection** Allows you to connect to the data store and disconnect from him, in addition, provides access to relevant transaction objects.

[Back To Index](#activex-data-objects-for-net)

<br>

### DbDataAdapter

**DbDataAdapter**Transfers data sets from the data store to the calling process and vice versa.

[Back To Index](#activex-data-objects-for-net)

<br>
