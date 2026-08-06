# Experiment 0: Introduction to SQL and MySQL

## Objective

- To understand the basics of SQL and its applications.
- To learn different categories of SQL commands.
- To install and set up MySQL.

---

# What is SQL?

**SQL (Structured Query Language)** is a standard language used to communicate with relational databases. It allows users to create databases, store data, retrieve information, update records, and manage database objects.

## Uses of SQL

- Creating and managing databases.
- Storing, updating, and deleting data.
- Retrieving information using queries.
- Managing user access and permissions.
- Maintaining relationships between tables.

---

# SQL Commands

SQL commands are divided into five categories:

1. DDL (Data Definition Language)
2. DML (Data Manipulation Language)
3. DQL (Data Query Language)
4. DCL (Data Control Language)
5. TCL (Transaction Control Language)

---

# 1. DDL (Data Definition Language)

DDL commands are used to create and modify database structures.

## CREATE

**Use:** Creates a new table or database.

**Syntax:**

```sql
CREATE TABLE table_name (
    column_name datatype
);
````

---

## ALTER

**Use:** Modifies an existing table.

**Syntax:**

```sql
ALTER TABLE table_name
ADD column_name datatype;
```

---

## DROP

**Use:** Deletes a table or database permanently.

**Syntax:**

```sql
DROP TABLE table_name;
```

---

## TRUNCATE

**Use:** Removes all records from a table while keeping its structure.

**Syntax:**

```sql
TRUNCATE TABLE table_name;
```

---

# 2. DML (Data Manipulation Language)

DML commands are used to manipulate data stored in tables.

## INSERT

**Use:** Adds new records.

**Syntax:**

```sql
INSERT INTO table_name
VALUES (value1, value2);
```

---

## UPDATE

**Use:** Modifies existing records.

**Syntax:**

```sql
UPDATE table_name
SET column_name=value
WHERE condition;
```

---

## DELETE

**Use:** Removes records.

**Syntax:**

```sql
DELETE FROM table_name
WHERE condition;
```

---

# 3. DQL (Data Query Language)

## SELECT

**Use:** Retrieves data from a database.

**Syntax:**

```sql
SELECT column_name
FROM table_name;
```

Example:

```sql
SELECT * FROM Student;
```

### Common Clauses

* **WHERE** - Filters records.
* **ORDER BY** - Sorts records.
* **GROUP BY** - Groups similar records.
* **HAVING** - Filters grouped results.
* **DISTINCT** - Removes duplicate values.

---

# 4. DCL (Data Control Language)

DCL commands manage database permissions.

## GRANT

**Use:** Gives privileges to users.

**Syntax:**

```sql
GRANT privilege
ON table_name
TO user_name;
```

---

## REVOKE

**Use:** Removes user privileges.

**Syntax:**

```sql
REVOKE privilege
ON table_name
FROM user_name;
```

---

# 5. TCL (Transaction Control Language)

TCL commands manage database transactions.

## COMMIT

Saves changes permanently.

```sql
COMMIT;
```

---

## ROLLBACK

Reverts changes.

```sql
ROLLBACK;
```

---

## SAVEPOINT

Creates a point for rollback.

```sql
SAVEPOINT savepoint_name;
```

---

# MySQL Installation Procedure

1. Download the MySQL Installer.
2. Run the installer and select the required setup type.
3. Install the required MySQL components.
4. Configure MySQL Server.
5. Set a password for the root user.
6. Complete the configuration process.
7. Open MySQL Workbench.
8. Connect using the MySQL credentials.
9. Verify installation using:

```sql
SHOW DATABASES;
```

If databases are displayed, MySQL installation is successful.

---

# Conclusion

SQL is an important language used for managing relational databases. It provides commands to create, modify, retrieve, and control data efficiently. MySQL provides a practical environment to execute SQL queries and work with databases.
