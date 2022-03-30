---
layout: default
title: MySQL Workbench tips
nav_order: 6
---

# MySQL Workbench Tips

Statements, clauses, and various datatypes in MySQL will often be highlighted in another color. \
Here is an example:

```sql
SELECT id, dob
FROM User
WHERE name = "Grace" AND dob > 20000000;
```

With MySQL Workbench, you can often troubleshoot your own errors, by highlighting over red_underlined text as can be seen in the example below.

```sql
SELECT *
FROM Reef
WHERE reefName IN [SELECT] // (1)

1. SELECT is not valid at this position for this server version, expecting FOR, LOCK, TABLE, VALUES, WITH, '('
```
