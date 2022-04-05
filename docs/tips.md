---
layout: default
title: MySQL Workbench tips
nav_order: 6
---

# MySQL Workbench Tips

## Query Display

Statements, clauses, and various datatypes in MySQL will often be highlighted in another color. \
Here is an example:

```sql
SELECT id, dob
FROM User
WHERE name = "Grace" AND dob > 20000000;
```

## Troubleshooting

With MySQL Workbench, you can often troubleshoot your own errors, by highlighting over red_underlined text as can be seen in the example below.

```sql
SELECT *
FROM Reef
WHERE reefName IN [SELECT] // (1)

1. SELECT is not valid at this position for this server version, expecting FOR, LOCK, TABLE, VALUES, WITH, '('
```

## Basic Data Types

### String Data Types

| Data type                   | Description                                                                                                                                                                                                                                                             |
|-----------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| CHAR(size)                  | A FIXED length string (can contain letters, numbers, and special characters). The size parameter specifies the column length in characters - can be from 0 to 255. Default is 1                                                                                         |
| VARCHAR(size)               | A VARIABLE length string (can contain letters, numbers, and special characters). The size parameter specifies the maximum column length in characters - can be from 0 to 65535                                                                                          |
| ENUM(val1, val2, val3, ...) | A string object that can have only one value, chosen from a list of possible values. You can list up to 65535 values in an ENUM list. If a value is inserted that is not in the list, a blank value will be inserted. The values are sorted in the order you enter them |

### Numeric Data Types

| Data type       | Description                                                                                                                                                        |
|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| BOOL            | Zero is considered as false, nonzero values are considered as true.                                                                                                |
| DOUBLE(size, d) | A normal-size floating point number. The total number of digits is specified in size. The number of digits after the decimal point is specified in the d parameter |
| INT             | A medium integer. Signed range is from -2147483648 to 2147483647. Unsigned range is from 0 to 4294967295.                                                          |

### Date and Time Data Types

| Data type     | Description                                                                                                                                                                                                                                                           |
|---------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| DATE          | A date. Format: YYYY-MM-DD. The supported range is from '1000-01-01' to '9999-12-31'                                                                                                                                                                                  |
| DATETIME(fsp) | A date and time combination. Format: YYYY-MM-DD hh:mm:ss. The supported range is from '1000-01-01 00:00:00' to '9999-12-31 23:59:59'. Adding DEFAULT and ON UPDATE in the column definition to get automatic initialization and updating to the current date and time |
| YEAR          | A year in four-digit format. Values allowed in four-digit format: 1901 to 2155, and 0000. MySQL 8.0 does not support year in two-digit format.                                                                                                                        |