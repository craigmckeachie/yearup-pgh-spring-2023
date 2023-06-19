## MySQL vs SQLite Workbook Differences

- use these [database examples](https://github.com/craigmckeachie/sqlite-examples)
- use [SQLite VS Code Extension](https://marketplace.visualstudio.com/items?itemName=alexcvzz.vscode-sqlite)

- use databasename;
  - doesn't work
  - instead use VS Code Command Palette > SQLite Use Database
- select \* from database.tablename
  - doesn't work
  - instead use VS Code Command Palette > SQLite Use Database
- SQL_SAFE_UPDATES (MySQL) not applicable to SQLite
- Now() (MySQL) = Date() (SQLite)
  - use in first INSERT example
- START TRANSACTION; COMMIT (MySQL) = BEGIN TRANSACTION; COMMIT; (SQLite)
- No easy way to create database diagrams. No VS Code Extension Supports. [More information](https://stackoverflow.com/questions/59654755/how-to-generate-sqlite-entity-relationship-diagram-from-database-file).
- AUTO_INCREMENT (MySQL) = AUTOINCREMENT (SQLite)
  - Create table example in SQLite
  ```sql
    CREATE TABLE advertisements (
    AdId INTEGER NOT NULL PRIMARY KEY AUTOINCREMENT,
    Title varchar(50) NOT NULL,
    MagicCode varchar(9),
    PercentOff float NOT NULL);
  ```
- Data Types supported by each database differ

## Comparison

- [Appropriate Uses](https://www.sqlite.org/whentouse.html)
- [Difference Between SQLite and MySQL](https://www.janbasktraining.com/blog/sqlite-vs-mysql/)

## Other Gotchas

- First join queries involving sakila customer and order tables cannot be run as examples because order table doesn't exist in sakila unless you create it manually
