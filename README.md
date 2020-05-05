# Docker-Commandsh

<img src="docker.png" height="150" alt="">

### Select

<br />

* Select all fields from table
```sql
SELECT * FROM <table_name>
```

* Select specific columns from table
```sql
SELECT <column_name1>, <column_name2> FROM <table_name>
```

* Select unique (non-duplicates) values from table
```sql
SELECT DISTINCT FROM <table_name>
```

* Get count
```sql
SELECT COUNT(<column_name> || *) FROM <table_name>
```
> Examples
```sql
SELECT COUNT(*) FROM t_users

SELECT COUNT(city) FROM t_users
```

* Select count of unique (non-duplicates) values from table
```sql
SELECT COUNT(DISTINCT <column_name> || *) FROM <table_name>
```

> Examples
```sql
SELECT COUNT(DISTINCT city) FROM t_users

SELECT COUNT(DISTINCT *) FROM t_users
```


### Search

<br />

* Search using string value (Only single quote allowed & case-sensitive)
```sql
SELECT * FROM <table_name> WHERE name = '<string>'
``` 

* Search using numeric values (with >, <, =, /)
```sql
SELECT * FROM <table_name> WHERE id = <numeric_value>

SELECT * FROM <table_name> WHERE age > <numeric_value>

SELECT * FROM <table_name> WHERE age < <numeric_value>

SELECT * FROM <table_name> WHERE interest / <numeric_value> = 0
```

* Search using date values
```sql
SELECT * FROM <table_name> WHERE date > '<YEAR-MONTH-DAY>'
```

> Example
```sql
SELECT * FROM users WHERE age > '1990-04-15'
```