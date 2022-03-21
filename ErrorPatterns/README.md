# Error Patterns

## Databases
### MySQL
- `(SQL syntax.*MySQL|Warning.*mysql_.*|MySqlException \\(0x|valid MySQL result|check the manual that corresponds to your (MySQL|MariaDB) server version|MySqlClient\\.|com\\.mysql\\.jdbc\\.exceptions)`
- `SQL syntax.*?MySQL`
- `Warning.*?mysqli?`
- `MySQLSyntaxErrorException`
- `valid MySQL result`
- `check the manual that (corresponds to|fits) your MySQL server version`
- `check the manual that (corresponds to|fits) your MariaDB server version`
- `check the manual that (corresponds to|fits) your Drizzle server version`
- `Unknown column '[^ ]+' in 'field list'`
- `com\\.mysql\\.jdbc`
- `Zend_Db_(Adapter|Statement)_Mysqli_Exception`
- `MySqlException`
- `Syntax error or access violation`

### PostgreSQL
- `(PostgreSQL.*ERROR|Warning.*\\Wpg_.*|valid PostgreSQL result|Npgsql\\.|PG::SyntaxError:|org\\.postgresql\\.util\\.PSQLException|ERROR:\\s\\ssyntax error at or near)`
- `PostgreSQL.*?ERROR"`
- `Warning.*?\\Wpg_`
- `valid PostgreSQL result`
- `Npgsql\\."`
- `PG::SyntaxError:`
- `org\\.postgresql\\.util\\.PSQLException`
- `ERROR:\\s\\ssyntax error at or near`
- `ERROR: parser: parse error at or near`
- `PostgreSQL query failed`
- `org\\.postgresql\\.jdbc`
- `PSQLException`

### MSSQL
- `(Driver.* SQL[\\-\\_\\ ]*Server|OLE DB.* SQL Server|\bSQL Server.*Driver|Warning.*mssql_.*|\bSQL Server.*[0-9a-fA-F]{8}|[\\s\\S]Exception.*\\WSystem\\.Data\\.SqlClient\\.|[\\s\\S]Exception.*\\WRoadhouse\\.Cms\\.|Microsoft SQL Native Client.*[0-9a-fA-F]{8})`
- `Driver.*? SQL[\\-\\_\\ ]*Server`
- `OLE DB.*? SQL Server`
- `\bSQL Server[^&lt;&quot;]+Driver`
- `Warning.*?\\W(mssql|sqlsrv)_`
- `\bSQL Server[^&lt;&quot;]+[0-9a-fA-F]{8}`
- `System\\.Data\\.SqlClient\\.SqlException`
- `(?s)Exception.*?\bRoadhouse\\.Cms\\.`
- `Microsoft SQL Native Client error '[0-9a-fA-F]{8}`
- `\\[SQL Server\\]`
- `ODBC SQL Server Driver`
- `ODBC Driver \\d+ for SQL Server`
- `SQLServer JDBC Driver"`
- `com\\.jnetdirect\\.jsql`
- `macromedia\\.jdbc\\.sqlserver`
- `Zend_Db_(Adapter|Statement)_Sqlsrv_Exception`
- `com\\.microsoft\\.sqlserver\\.jdbc`
- `SQL(Srv|Server)Exception`

### Oracle
`(\\bORA-\\d{5}|Oracle error|Oracle.*Driver|Warning.*\\Woci_.*|Warning.*\\Wora_.*)`

### IBMDB2
`(CLI Driver.*DB2|DB2 SQL error|\\bdb2_\\w+\\(|SQLSTATE.+SQLCODE)`

### Informix
`(Exception.*Informix)`

### SQLite
`(SQLite\\/JDBCDriver|SQLite.Exception|System.Data.SQLite.SQLiteException|Warning.*sqlite_.*|Warning.*SQLite3::|\\[SQLITE_ERROR\\])`

### SAPDB
`(SQL error.*POS([0-9]+).*|Warning.*maxdb.*)`

### Sybase
`(Warning.*sybase.*|Sybase message|Sybase.*Server message.*|SybSQLException|com\\.sybase\\.jdbc)`

### Ingress
`(Warning.*ingres_|Ingres SQLSTATE|Ingres\\W.*Driver)`

### Frontbase
`(Exception (condition )?\\d+. Transaction rollback.)`

### HSQLDB
`(org\\.hsqldb\\.jdbc|Unexpected end of command in statement \\[|Unexpected token.*in statement \\[)`
