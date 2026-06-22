# PostgreSQL Cheatsheet

Each student will complete the Description and Example sections for the SQL clause assigned to them.

For each clause:

1. In the **Description**, explain what the clause does in plain language.main
2. In the **Example**, write a working SQL statement that shows how the clause is used (like the `SELECT and `CREATE TABLE` examples below).
3. As a reference, `SELECT` and `CREATE TABLE` are already done for you.

---

### 1. `SELECT`
   
**Description:** `SELECT *` returns all columns from the provided table. You can also do `SELECT column_name_1, column_name_2` to return specific columns from the provided table.

**Example:**

```sql
SELECT *
FROM movies;
```

### 2. `CREATE TABLE`

**Description:** `CREATE TABLE` creates a new table in a database. It allows one to specify the name of the table, the name of each column, and each column's data type in the table.

**Example:**

```sql
CREATE TABLE friends (
  friend_id SERIAL PRIMARY KEY,
  name VARCHAR,
  birthday DATE
);
```

### 3. `INSERT INTO` — assigned to: Arianne

**Description:** 

**Example:**

```sql

```


### 4. `UPDATE` — assigned to: Carlotta

**Description:** `UPDATE` is used to modify existing data in a table. It changes the value of one or more columns for rows that match a specified condition. It is important to set the 'WHERE' clause when updating so that every row in the table is affected by the change.

**Example:**

```sql
UPDATE friends
SET city = 'Novato'
WHERE name = 'Carlotta';
```

### 5. `DELETE FROM` — assigned to: Hailey

**Description:**
Removes one or more rows from a table based on a condition.
**Example:**

```sql
DELETE FROM table_name
WHERE condition;
```

### 6. `GROUP BY` — assigned to: Jana

**Description:**

**Example:**

```sql

```

### 7. `ORDER BY` — assigned to: Zesty Pepper

**Description:**

**Example:**

```sql

```

### 8. `INNER JOIN` — assigned to: Morgan

**Description:**

An INNER JOIN returns only the rows that have matching values in both tables. Rows without a match in either table are excluded from the result.

**Example:**

```sql
SELECT
    customers.customer_name,
    orders.order_id
FROM customers
INNER JOIN orders
    ON customers.customer_id = orders.customer_id;
```

### 9. `LIMIT` — assigned to: Seth
**Description:**

**Example:**

```sql

```

### 10. `ON CONFLICT` — assigned to: Shirley

**Description:**

**Example:**

```sql

```

### 11. `LIKE` — assigned to: Ysabel

**Description:**

**Example:**

```sql

```

### 12. `COUNT` — assigned to Phil

**Description:** Counts the number of rows in a column

**Example:**

```sql
SELECT COUNT(*)
FROM fake_apps
WHERE price = 0;
```
