# Structured Query Language

## Create Table

**Format**: CREATE TABLE `<table>` (`<columns>`)

```sql
CREATE TABLE users (username, password)
```

<p align="center">
  <img src="https://github.com/thespcrewroy/Pwn.College/blob/main/assets/create-table.png" alt="Demo" width="500" />
</p>

## Insert Into

**Format**: INSERT INTO `<table>` VALUES (`<values>`)

```sql
INSERT INTO users VALUES ("admin", "admin")
INSERT INTO users VALUES ("connor", "password123")
INSERT INTO users VALUES ("kanak", "hunter2")
```

<p align="center">
  <img src="https://github.com/thespcrewroy/Pwn.College/blob/main/assets/insert-into.png" alt="Demo" width="500" />
</p>

## Select

**Format**: SELECT `<column>` FROM `<table>` WHERE `<conditions>`

```sql
SELECT username, password FROM users
SELECT username FROM users
SELECT * FROM users
SELECT * FROM users WHERE username = "admin"
SELECT * FROM users WHERE username = "admin" and password = "password"
SELECT * FROM users WHERE username = "admin" and password = "admin"
```

<p align="center">
  <img src="https://github.com/thespcrewroy/Pwn.College/blob/main/assets/select6.png" alt="Demo" width="500" />
</p>

## Delete

**Format**: DELETE FROM `<table>` WHERE `<conditions>`

```sql
DELETE FROM users WHERE username = "kanak"
```

<p align="center">
  <img src="https://github.com/thespcrewroy/Pwn.College/blob/main/assets/delete.png" alt="Demo" width="500" />
</p>

## Update

**Format**: UPDATE `<table>` SET `<assignments>` WHERE `<conditions>`

```sql
UPDATE users SET password = "password456" WHERE username = "connor"
```

<p align="center">
  <img src="https://github.com/thespcrewroy/Pwn.College/blob/main/assets/update.png" alt="Demo" width="500" />
</p>

## Union

**Format**: `<select>` UNION `<select>`

```sql
SELECT username FROM users UNION SELECT password FROM users
```

<p align="center">
  <img src="https://github.com/thespcrewroy/Pwn.College/blob/main/assets/union.png" alt="Demo" width="500" />
</p>

## Retreive All Tables in SQLite Database Schema

**Format**: SELECT `<tbl_name>` FROM sqlite_master

<p align="center">
  <img src="https://github.com/thespcrewroy/Pwn.College/blob/main/assets/schema-table.png" alt="Demo" width="500" />
</p>

## Drop Table

**Format**: DROP TABLE `<table>`

```sql
DROP TABLE users
```

<p align="center">
  <img src="https://github.com/thespcrewroy/Pwn.College/blob/main/assets/drop-table.png" alt="Demo" width="500" />
</p>
