## The latest version[2026.5.0](https://plugins.jetbrains.com/plugin/19161-database-tool)
**Databee** is a database client that lives in your IDE: browse your schemas, write SQL the editor understands, run it, and edit the results in place. Works in IntelliJ IDEA and other IntelliJ-based IDEs.

**Databases:** MySQL, MariaDB, TiDB, and OceanBase (MySQL mode); PostgreSQL, CockroachDB, and YugabyteDB; Oracle, Microsoft SQL Server, SQLite, and ClickHouse; MongoDB; Redis and Valkey.

**SQL editor** — every dialect has its own parser, so the editor reads what you wrote instead of guessing:

-   Completion of tables, columns, aliases and CTEs from the schema you are connected to
-   Table and column names the connected data source does not have are marked in the editor, plus an inspection for checking a whole directory at once
-   `DELETE` / `UPDATE` without a `WHERE` is flagged while you type; `TRUNCATE` and `DROP` are confirmed before they run
-   Formatting, code folding, comment/uncomment, live templates, Oracle PL/SQL packages (`.pkb` / `.pks`)
-   SQL inside Java, Kotlin and XML string literals gets the same highlighting and completion, MyBatis mappers included
-   Ctrl+Enter runs the statement under the caret, and every top-level statement has a run icon in the gutter
-   The dialect is a project setting and can be overridden per file

**Data**

-   Browse databases, schemas, tables, views, columns and indexes
-   Edit result-grid cells, insert and delete rows, then submit the DML; paging, sorting and filtering included
-   Create / alter / rename / drop / truncate, with the SQL shown before it is applied
-   Export a query or a table as CSV, Excel, JSON, or as `INSERT` / `UPDATE` statements; import CSV
-   Run a whole `.sql` file against the connection you pick

**Connections**

-   JDBC drivers download from Maven in one click, or point at your own jars
-   SSH tunnels, SSL with custom CA and client certificates
-   Passwords live in the IDE password safe, never in the project files

**MCP** (IDE 2025.2+): `dbtool_*` tools for connections, metadata, query and execute, export/import and drivers — enable them in Settings → Tools → MCP Server. Passwords are never returned.

How to use: open the Databee window → add a data source → open a SQL file → pick the connection → Ctrl+Enter.

[GitHub](https://github.com/mbtsp/Databae-Tool) · [Issues](https://github.com/mbtsp/Databae-Tool/issues)

idea Database plugin
demo:
 ![分页](https://user-images.githubusercontent.com/31949635/179384725-3de56feb-0d99-4a9f-a649-14ff9e59f4da.gif)
 ![dropAndDrag](https://user-images.githubusercontent.com/31949635/233034183-83c65d76-9463-4270-902d-e586d13dcc4c.gif)

