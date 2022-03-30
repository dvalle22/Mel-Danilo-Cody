---
layout: default
title: Introduction
nav_order: 1
description: "Introduction to MySQL Workbench User Guide."
permalink: /
---

# MySQL Workbench User Guide
{: .fs-9 }

An user guide for frequently performed tasks on MySQL Workbench.
{: .fs-6 .fw-300 }

[Get started](#introduction){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/dvalle22/Mel-Danilo-Cody){: .btn .fs-5 .mb-4 .mb-md-0 }

---

## Introduction

Welcome! MySQL Workbench User Guide is a step-by-step instruction guide for frequently performed tasks on MySQL Workbench. The documentation for each task can be completed sequentially and takes readers through creating new schemas to writing and executing MySQL statements.

MySQL Workbench (or just Workbench) is an application software for database design using the popular relational database management system, MySQL. A powerful tool for software developers, Workbench provides a visual environment to create, execute, and optimize databases through its graphical user interface or with queries written in the SQL programming language.

## Intended User Groups
The user documentation in MySQL Workbench User Guide is intended for the following users:
- New users who want to start learning MySQL
- Returning users who want to review MySQL's commands

## Software Requirements
- MySQL
- MySQL Workbench 8.0 CE

## Prerequisites
- Have access to a working computer and ability to performs basic computer-oriented tasks
- Have bility to navigate yourself about various interfaces, given a set of instructions
- Already set up a MySQL connection (If not, please refer to our [Set Up Guide](#procedures-overview))

## Why MySQL
- MySQL is one of the easiest and most secure ways to maintain and update a database.
- MySQL provides high-performance at a low cost. In fact, MySQL community edition is free!
- Flexible and usable across all major platforms, including: Windows, Mac, Linux, Ubuntu and more.

## Procedures Overview
[MySQL Workbench setup](#introduction)

[Schema Setup and Adding Tables](#introduction)

[Query to Modify Data](#introduction)

[Query to Display Data](#introduction)

## Typographical Conventions
    
### Warning Messages

    📖: Additional information
    > This icon notes where additional information, such as notes and shortcut, is provided.
    
    ⚠️: Dangerous action
    > This icon notes where a dangerous action could take place.
    
### MySQL Workbench Tips
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
