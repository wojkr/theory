# ActiveX Data Objects for .NET

[DbDataReader](#dbdatareader)
[DbDataCommand](#dbdatacommand)
[DbDataConnection](#dbdataconnection)
[DbDataAdapter](#dbdataadapter)

[ExecuteNonQuery](#executenonquery)
[ExecuteReader](#executereader)
[ExecuteScalar](#executescalar)

### DbDataReader

**DbDataReader** Provides read-only data access in the forward direction with a server-side cursor.

[Back To Index](#index)

<br>

### DbDataCommand

**DbDataCommand** Represents a SQL query or stored procedure and also provide access to the read object provider-specific data.

[Back To Index](#index)

<br>

### DbDataConnection

**DbDataConnection** Allows you to connect to the data store and disconnect from him, in addition, provides access to relevant transaction objects.

[Back To Index](#index)

<br>

### DbDataAdapter

**DbDataAdapter**Transfers data sets from the data store to the calling process and vice versa.

[Back To Index](#index)

<br>

### ExecuteScalar()

**ExecuteScalar()** method of the DbCommand class is the best suited when you have aggregate SQL functions in a `SELECT` statement.

[Back To Index](#index)

<br>

### ExecuteReader()

**ExecuteReader()** method of the `DbCommand` class is the best suited when you execute a `SELECT` query and return a reader object that wraps a readonly, forward-only cursor.

[Back To Index](#index)

<br>

### ExecuteNonQuery()

**ExecuteNonQuery** method of the `DbCommand` class is the best suited when you execute non-SELECT commands, such as SQL commands that **insert, delete, update** records or execute datadefinition commands that `create`, `alter`, or `delete` database objects (such as tables, indexes, constraints, and so on).

[Back To Index](#index)

<br>

### Classes that make up a data provider include:

- `DbCommand`
- `DbDataReader`
- `DbConnection`
- `DbDataAdapter`

[Back To Index](#index)
