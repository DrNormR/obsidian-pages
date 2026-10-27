---
{"dg-publish":true,"permalink":"/newman/bsad-6434-data-programming/module-3-database-command-line/database-command-line-instructor-notes/","noteIcon":""}
---


---

# ✔️To Do

- [ ] [item]

---

# ❓Questions

---

# 🔗Links

---

# Module: Database Command Line - Instructor Notes

**Date:** 2026-10-12

**Tags:** #module #newman

---

> [!example]- Module Welcome
> *- [Record a short video welcoming them and giving a preview of upcoming assignments ]*
> - Notes for video:

> [!example]- Announcements
> *- [Copy/paste announcements from Canvas]*

> [!example]- Reading Assignments
> *- Template for Canvas:*
> 
> The reading assignment for this module comes from [ ==insert== ]. A PDF is attached, as well as the link to the website.
> 
> - ==- PDF Insert==
> - ==- URL here==
> 
> License: This work is licensed under a [Creative Commons Attribution-ShareAlike 3.0 License](http://creativecommons.org/licenses/by-sa/3.0/)

> [!example]- Links

---

## 🎥Video

### Welcome Video

[paste embed code here for embedded video]

```
[paste embed code here for copying]
```

[paste video link here]

## 🎙️Notes / Lecture

### Instructor Notes - Section 1

#### [SQL Server Command Line Basics] Video

<iframe width="640" height="347" src="https://www.loom.com/embed/9c3a966be9194531bb2d808ba3c0b864?sid=86c55f99-4087-4d48-a1b4-1d543e614a58" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

```
<iframe width="640" height="347" src="https://www.loom.com/embed/9c3a966be9194531bb2d808ba3c0b864?sid=86c55f99-4087-4d48-a1b4-1d543e614a58" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>
```

[https://www.loom.com/share/9c3a966be9194531bb2d808ba3c0b864?sid=65434745-cb65-46f1-9e7b-e8d4e4cc49a6](https://www.loom.com/share/9c3a966be9194531bb2d808ba3c0b864?sid=65434745-cb65-46f1-9e7b-e8d4e4cc49a6)

#### MS SQL Basics
### Database Operations

```sql
CREATE DATABASE Norman;
GO
```
- Creates a new database

![Pasted image 20261027172945.png](/img/user/Newman/BSAD%206434%20Data%20Programming/Module%203%20-%20Database%20Command%20Line/~media/Pasted%20image%2020261027172945.png)

```sql
SELECT name FROM sys.databases;
GO
```
- Shows all current databases on the server

```sql
USE Norman;
GO
```
- Sets the active database context to `Norman`

![Pasted image 20261027173001.png](/img/user/Newman/BSAD%206434%20Data%20Programming/Module%203%20-%20Database%20Command%20Line/~media/Pasted%20image%2020261027173001.png)

### Table Management (DDL)

```sql
CREATE TABLE table1 (
    user_id VARCHAR(50)
);
GO
```

```sql
SELECT name FROM sys.tables;
GO
```
- Lists all tables in the current database

![Pasted image 20261027173016.png](/img/user/Newman/BSAD%206434%20Data%20Programming/Module%203%20-%20Database%20Command%20Line/~media/Pasted%20image%2020261027173016.png)

```sql
EXEC sp_help 'table1';
GO
```
- Displays table schema details (columns, types, attributes)

```sql
CREATE TABLE employees (
    employee_id INT IDENTITY(1,1) PRIMARY KEY,
    first_name VARCHAR(50) NOT NULL,
    last_name VARCHAR(50) NOT NULL,
    bio TEXT,
    salary DECIMAL(10,2) NOT NULL,
    is_active BIT DEFAULT 1,
    hire_date DATE
);
GO
```
- Identity 1,1 is an auto increment primary key 

```sql
EXEC sp_help 'employees';
GO
```
- Displays table definition and primary key constraints

![Pasted image 20261027173048.png](/img/user/Newman/BSAD%206434%20Data%20Programming/Module%203%20-%20Database%20Command%20Line/~media/Pasted%20image%2020261027173048.png)
### Data Manipulation (DML)

```sql
INSERT INTO employees (first_name, last_name, bio, salary, is_active)
VALUES ('Alice', 'Johnson', 'Experienced secretary', 45332.00, 1);
GO
```

- Notice here that I don't insert the ID number because it's auto incremented

```sql
INSERT INTO employees (first_name, last_name)
VALUES ('The', 'Rock');
GO
```
- Fails with an error: `salary` cannot be NULL because the column has a `NOT NULL` constraint

![Pasted image 20261027173110.png](/img/user/Newman/BSAD%206434%20Data%20Programming/Module%203%20-%20Database%20Command%20Line/~media/Pasted%20image%2020261027173110.png)

```sql
INSERT INTO employees (first_name, last_name, bio, salary)
VALUES ('The', 'Rock', NULL, 99999.99);
GO
```

```sql
SELECT * FROM employees;
GO
```
- Queries and displays all records from the `employees` table

![Pasted image 20261027173136.png](/img/user/Newman/BSAD%206434%20Data%20Programming/Module%203%20-%20Database%20Command%20Line/~media/Pasted%20image%2020261027173136.png)

```sql
DELETE FROM employees;
GO
```
- Deletes all records from the `employees` table

### Instructor Notes - Section 2

#### [topic] Video

[paste embed code here for embedded video]

```
[paste embed code here for copying]
```

[paste video link here]


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



### 🟠 Section 2 -

</div></div>


### Instructor Notes - Section 3

#### [topic] Video

[paste embed code here for embedded video]

```
[paste embed code here for copying]
```

[paste video link here]


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



### 🟩 Section 3 -

</div></div>


### Instructor Notes - Section 4

#### [topic] Video

[paste embed code here for embedded video]

```
[paste embed code here for copying]
```

[paste video link here]


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



### 🟥 Section 4 -

</div></div>


### Instructor Notes - Section 5

#### [topic] Video

[paste embed code here for embedded video]

```
[paste embed code here for copying]
```

[paste video link here]


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



### 🟣 Section 5 -

---


</div></div>


---


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



## 🧬 Programming Time 

| ![[Pasted image 20260223193209.png\|350]] | ![[Pasted image 20260224181940.png\|350]] |
| ----------------------------------------- | ----------------------------------------- |

> [!example]- Code: [ ]
> ```python
> #reading a CSV with headers named x1, x2, and y
> #returns x (2-D array) and y (1-D array)
> def load_x1x2y(csv_path: Path) -> Tuple[np.ndarray, np.ndarray]:
>     """Load x1, x2, and y columns from a CSV with headers x1,x2,y."""
>     data = np.genfromtxt(csv_path, delimiter=",", names=True, dtype=float)
> %% 
>     #make sure required headers exist
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
>     x1 = np.asarray(data["x1"], dtype=float)
>     x2 = np.asarray(data["x2"], dtype=float)
>     y = np.asarray(data["y"], dtype=float)
> 
>     #basic shape checks
>     if x1.ndim != 1 or x2.ndim != 1 or y.ndim != 1:
>         raise ValueError("x1, x2, y must be 1-D arrays.")
>     if len(x1) != len(x2) or len(x1) != len(y):
>         raise ValueError("x1, x2, and y must be the same length.")
> 
>     #stack x1 and x2 into a 2-D feature matrix
>     X = np.column_stack([x1, x2]).astype(float)
>     return X, y %%
> ```

> [!info]- Code Explanation
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```

> [!example]- Code: [ ]
> ```python
> #reading a CSV with headers named x1, x2, and y
> #returns x (2-D array) and y (1-D array)
> def load_x1x2y(csv_path: Path) -> Tuple[np.ndarray, np.ndarray]:
>     """Load x1, x2, and y columns from a CSV with headers x1,x2,y."""
>     data = np.genfromtxt(csv_path, delimiter=",", names=True, dtype=float)
> %% 
>     #make sure required headers exist
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
>     x1 = np.asarray(data["x1"], dtype=float)
>     x2 = np.asarray(data["x2"], dtype=float)
>     y = np.asarray(data["y"], dtype=float)
> 
>     #basic shape checks
>     if x1.ndim != 1 or x2.ndim != 1 or y.ndim != 1:
>         raise ValueError("x1, x2, y must be 1-D arrays.")
>     if len(x1) != len(x2) or len(x1) != len(y):
>         raise ValueError("x1, x2, and y must be the same length.")
> 
>     #stack x1 and x2 into a 2-D feature matrix
>     X = np.column_stack([x1, x2]).astype(float)
>     return X, y %%
> ```

> [!info]- Code Explanation
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```

> [!example]- Code: [ ]
> ```python
> #reading a CSV with headers named x1, x2, and y
> #returns x (2-D array) and y (1-D array)
> def load_x1x2y(csv_path: Path) -> Tuple[np.ndarray, np.ndarray]:
>     """Load x1, x2, and y columns from a CSV with headers x1,x2,y."""
>     data = np.genfromtxt(csv_path, delimiter=",", names=True, dtype=float)
> %% 
>     #make sure required headers exist
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
>     x1 = np.asarray(data["x1"], dtype=float)
>     x2 = np.asarray(data["x2"], dtype=float)
>     y = np.asarray(data["y"], dtype=float)
> 
>     #basic shape checks
>     if x1.ndim != 1 or x2.ndim != 1 or y.ndim != 1:
>         raise ValueError("x1, x2, y must be 1-D arrays.")
>     if len(x1) != len(x2) or len(x1) != len(y):
>         raise ValueError("x1, x2, and y must be the same length.")
> 
>     #stack x1 and x2 into a 2-D feature matrix
>     X = np.column_stack([x1, x2]).astype(float)
>     return X, y %%
> ```

> [!info]- Code Explanation
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```

> [!example]- Code: [ ]
> ```python
> #reading a CSV with headers named x1, x2, and y
> #returns x (2-D array) and y (1-D array)
> def load_x1x2y(csv_path: Path) -> Tuple[np.ndarray, np.ndarray]:
>     """Load x1, x2, and y columns from a CSV with headers x1,x2,y."""
>     data = np.genfromtxt(csv_path, delimiter=",", names=True, dtype=float)
> %% 
>     #make sure required headers exist
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
>     x1 = np.asarray(data["x1"], dtype=float)
>     x2 = np.asarray(data["x2"], dtype=float)
>     y = np.asarray(data["y"], dtype=float)
> 
>     #basic shape checks
>     if x1.ndim != 1 or x2.ndim != 1 or y.ndim != 1:
>         raise ValueError("x1, x2, y must be 1-D arrays.")
>     if len(x1) != len(x2) or len(x1) != len(y):
>         raise ValueError("x1, x2, and y must be the same length.")
> 
>     #stack x1 and x2 into a 2-D feature matrix
>     X = np.column_stack([x1, x2]).astype(float)
>     return X, y %%
> ```

> [!info]- Code Explanation
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```

> [!example]- Code: [ ]
> ```python
> #reading a CSV with headers named x1, x2, and y
> #returns x (2-D array) and y (1-D array)
> def load_x1x2y(csv_path: Path) -> Tuple[np.ndarray, np.ndarray]:
>     """Load x1, x2, and y columns from a CSV with headers x1,x2,y."""
>     data = np.genfromtxt(csv_path, delimiter=",", names=True, dtype=float)
> %% 
>     #make sure required headers exist
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
>     x1 = np.asarray(data["x1"], dtype=float)
>     x2 = np.asarray(data["x2"], dtype=float)
>     y = np.asarray(data["y"], dtype=float)
> 
>     #basic shape checks
>     if x1.ndim != 1 or x2.ndim != 1 or y.ndim != 1:
>         raise ValueError("x1, x2, y must be 1-D arrays.")
>     if len(x1) != len(x2) or len(x1) != len(y):
>         raise ValueError("x1, x2, and y must be the same length.")
> 
>     #stack x1 and x2 into a 2-D feature matrix
>     X = np.column_stack([x1, x2]).astype(float)
>     return X, y %%
> ```

> [!info]- Code Explanation
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```

> [!example]- Code: [ ]
> ```python
> #reading a CSV with headers named x1, x2, and y
> #returns x (2-D array) and y (1-D array)
> def load_x1x2y(csv_path: Path) -> Tuple[np.ndarray, np.ndarray]:
>     """Load x1, x2, and y columns from a CSV with headers x1,x2,y."""
>     data = np.genfromtxt(csv_path, delimiter=",", names=True, dtype=float)
> %% 
>     #make sure required headers exist
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
>     x1 = np.asarray(data["x1"], dtype=float)
>     x2 = np.asarray(data["x2"], dtype=float)
>     y = np.asarray(data["y"], dtype=float)
> 
>     #basic shape checks
>     if x1.ndim != 1 or x2.ndim != 1 or y.ndim != 1:
>         raise ValueError("x1, x2, y must be 1-D arrays.")
>     if len(x1) != len(x2) or len(x1) != len(y):
>         raise ValueError("x1, x2, and y must be the same length.")
> 
>     #stack x1 and x2 into a 2-D feature matrix
>     X = np.column_stack([x1, x2]).astype(float)
>     return X, y %%
> ```

> [!info]- Code Explanation
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```

> [!example]- Code: [ ]
> ```python
> #reading a CSV with headers named x1, x2, and y
> #returns x (2-D array) and y (1-D array)
> def load_x1x2y(csv_path: Path) -> Tuple[np.ndarray, np.ndarray]:
>     """Load x1, x2, and y columns from a CSV with headers x1,x2,y."""
>     data = np.genfromtxt(csv_path, delimiter=",", names=True, dtype=float)
> %% 
>     #make sure required headers exist
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
>     x1 = np.asarray(data["x1"], dtype=float)
>     x2 = np.asarray(data["x2"], dtype=float)
>     y = np.asarray(data["y"], dtype=float)
> 
>     #basic shape checks
>     if x1.ndim != 1 or x2.ndim != 1 or y.ndim != 1:
>         raise ValueError("x1, x2, y must be 1-D arrays.")
>     if len(x1) != len(x2) or len(x1) != len(y):
>         raise ValueError("x1, x2, and y must be the same length.")
> 
>     #stack x1 and x2 into a 2-D feature matrix
>     X = np.column_stack([x1, x2]).astype(float)
>     return X, y %%
> ```

> [!info]- Code Explanation
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```

> [!example]- Code: [ ]
> ```python
> #reading a CSV with headers named x1, x2, and y
> #returns x (2-D array) and y (1-D array)
> def load_x1x2y(csv_path: Path) -> Tuple[np.ndarray, np.ndarray]:
>     """Load x1, x2, and y columns from a CSV with headers x1,x2,y."""
>     data = np.genfromtxt(csv_path, delimiter=",", names=True, dtype=float)
> %% 
>     #make sure required headers exist
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
>     x1 = np.asarray(data["x1"], dtype=float)
>     x2 = np.asarray(data["x2"], dtype=float)
>     y = np.asarray(data["y"], dtype=float)
> 
>     #basic shape checks
>     if x1.ndim != 1 or x2.ndim != 1 or y.ndim != 1:
>         raise ValueError("x1, x2, y must be 1-D arrays.")
>     if len(x1) != len(x2) or len(x1) != len(y):
>         raise ValueError("x1, x2, and y must be the same length.")
> 
>     #stack x1 and x2 into a 2-D feature matrix
>     X = np.column_stack([x1, x2]).astype(float)
>     return X, y %%
> ```

> [!info]- Code Explanation
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```

> [!example]- Code: [ ]
> ```python
> #reading a CSV with headers named x1, x2, and y
> #returns x (2-D array) and y (1-D array)
> def load_x1x2y(csv_path: Path) -> Tuple[np.ndarray, np.ndarray]:
>     """Load x1, x2, and y columns from a CSV with headers x1,x2,y."""
>     data = np.genfromtxt(csv_path, delimiter=",", names=True, dtype=float)
> %% 
>     #make sure required headers exist
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
>     x1 = np.asarray(data["x1"], dtype=float)
>     x2 = np.asarray(data["x2"], dtype=float)
>     y = np.asarray(data["y"], dtype=float)
> 
>     #basic shape checks
>     if x1.ndim != 1 or x2.ndim != 1 or y.ndim != 1:
>         raise ValueError("x1, x2, y must be 1-D arrays.")
>     if len(x1) != len(x2) or len(x1) != len(y):
>         raise ValueError("x1, x2, and y must be the same length.")
> 
>     #stack x1 and x2 into a 2-D feature matrix
>     X = np.column_stack([x1, x2]).astype(float)
>     return X, y %%
> ```

> [!info]- Code Explanation
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```
> If your CSV is missing any of these headers it'll throw a ValueError — make sure x1, x2, and y are all present.
> ```python
>     needed = {"x1", "x2", "y"}
>     if data.dtype.names is None or not needed.issubset(set(data.dtype.names)):
>         raise ValueError("CSV must have headers: x1,x2,y")
> ```


</div></div>


---

## Assessments


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



# Quiz

> [!question]- Quiz Instructions
> *Instructions for Canvas:*
>
> - This is a short quiz 
> - The quiz will give one question at a time
> - This quiz has a 20 minute time limit
> - You have 2 attempts at this quiz
> - Your grade will be the average of the two attempts
> - You will be able to see the correct answers after the quiz
> 
> - ==- PDF Insert==
> - ==- URL here==
> 
> *Questions*
> - [paste here]

## Quiz Questions


</div></div>


---

## Discussion

<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



# Discussion: [topic]

[Topic description]

Please respond to 2 classmates for this discussion.


</div></div>


---


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



# Assignments

---

## Assignment: [ ]

[directions]

<u>Submission Instructions</u>

- You must submit a Word/PDF/RTF/other document
- You must submit a Loom video

> [!info]- Rubric 📊
> #### **Content** (20 pts)
> **25 pts — Proficient**
> - The content is thorough and accurate.
> - ==specific comments here==
> **15 pts — Needs Improvement**
> - The content had some missing elements.
> **0 pts — Not Evident**
> - The content had major inaccuracies.
> 
> ---
>
> #### **Images** (20 pts)
> **10 pts — Proficient**
> - Required images are present and relevant.
> - ==specific comments here==
> **6 pts — Needs Improvement**
> - Required images are present but relevance is unclear.
> **0 pts — Not Evident**
> - No images present.
> 
> ---
>
> #### **Video** (20 pts)
> **50 pts — Proficient**
> - The video is effective and professional.
> - ==specific comments here==
> **30 pts — Needs Improvement**
> - The video has some issues.
> **0 pts — Not Evident**
> - No video submitted.

> [!info]- Assignment Notes 📝
> - [ notes here ]

> [!info]- Assignment Answer ❓
> - [ picture/text output ]

> [!info]- Other
> inside here:
> - misc

---

## Assignment: [ Concept ] Notebook

Access the following course on LinkedInLearning:

- ==[course title]==
- ==[URL]==

You need to complete the following sections:

- [ ] Section 1
- [ ] Section 2

==[picture of the course player]==

As you complete the course, keep a notebook of your progress with screenshots of concepts along with your explanations of the concepts. Specific items to include are listed below:

<u>Section Title</u>

<u>Section Title</u>

Along with the screenshots, write a short explanation of what is happening in the screenshot.

<u>Loom Video</u>

- Submit a very brief video (around 1 minute) showing me your notebook and highlighting the most important concept from the module

<u>Submission Instructions</u>

- You must submit a Word/PDF/RTF/other document
- You must submit a Loom video

---

> [!info]- Rubric 📊
> #### **Content** (20 pts)
> **25 pts — Proficient**
> - The content is thorough and accurate.
> - ==specific comments here==
> **15 pts — Needs Improvement**
> - The content had some missing elements.
> **0 pts — Not Evident**
> - The content had major inaccuracies.
> 
> ---
>
> #### **Images** (20 pts)
> **10 pts — Proficient**
> - Required images are present and relevant.
> - ==specific comments here==
> **6 pts — Needs Improvement**
> - Required images are present but relevance is unclear.
> **0 pts — Not Evident**
> - No images present.
> 
> ---
>
> #### **Video** (20 pts)
> **50 pts — Proficient**
> - The video is effective and professional.
> - ==specific comments here==
> **30 pts — Needs Improvement**
> - The video has some issues.
> **0 pts — Not Evident**
> - No video submitted.

> [!info]- Assignment Notes 📝
> - [ notes here ]

> [!info]- Assignment Answer ❓
> - [ picture/text output ]

> [!info]- Other
> inside here:
> - misc

---

## Assignment: Programming Notebook

Access the following course on LinkedInLearning:

- ==[course title]==
- ==[URL]==

You need to complete the following sections:

- [ ] Section 1
- [ ] Section 2

==[picture of the course player]==

As you complete the course, keep a notebook of your progress with screenshots of successful item completions, including the following:

<u>Section Title</u>

<u>Section Title</u>

Along with the screenshots, write a short explanation of what is happening in the screenshot.

<u>Loom Video</u>

- Submit a very brief video (around 1 minute) showing the end state of your program after the last tutorial and give a very brief explanation about what's going on.

<u>Submission Instructions</u>

- You must submit a Word/PDF/RTF/other document
- You must submit a Loom video

---

> [!info]- Rubric 📊
> #### **Content** (20 pts)
> **25 pts — Proficient**
> - The content is thorough and accurate.
> - ==specific comments here==
> **15 pts — Needs Improvement**
> - The content had some missing elements.
> **0 pts — Not Evident**
> - The content had major inaccuracies.
> 
> ---
>
> #### **Images** (20 pts)
> **10 pts — Proficient**
> - Required images are present and relevant.
> - ==specific comments here==
> **6 pts — Needs Improvement**
> - Required images are present but relevance is unclear.
> **0 pts — Not Evident**
> - No images present.
> 
> ---
>
> #### **Video** (20 pts)
> **50 pts — Proficient**
> - The video is effective and professional.
> - ==specific comments here==
> **30 pts — Needs Improvement**
> - The video has some issues.
> **0 pts — Not Evident**
> - No video submitted.

> [!info]- Assignment Notes 📝
> - [ notes here ]

> [!info]- Assignment Answer ❓
> - [ picture/text output ]

> [!info]- Other
> inside here:
> - misc

---

> [!quote]- ChatGPT Assignment Ideas


</div></div>

