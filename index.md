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

Welcome! MySQL Workbench User Guide is a step-by-step instruction guide for frequently performed tasks on MySQL Workbench. The documentation for each task can be completed sequentially and guides users through [task1], [task2], and [task3].

MySQL Workbench (or just Workbench) is an application software for database design using the popular relational database management system, MySQL. A powerful tool for software developers, Workbench provides a visual environment to create, execute, and optimize databases through its graphical user interface or with queries written in the SQL programming language.


## Intended User Groups
The user documentation in MySQL Workbench User Guide is intended for the following users:
- New users who want to start learning MySQL
- Returning users who want to review MySQL's commands

## Software Requirements
- MySQL
- MySQL Workbench 8.0 CE

## Prerequisite
- Access to a working computer and ability to performs basic computer-oriented tasks
- Ability to navigate yourself about various interfaces, given a set of instructions

## Why MySQL
- MySQL is one of the easiest and most secure ways to maintain and update a database.
- MySQL provides high-performance at a low cost. In fact, MySQL community edition is free!
- Flexible and usable across all major platforms, including: Windows, Mac, Linux, Ubuntu and more.

## Procedures Overview
- **Schema Setup and Adding Tables**
- **Writing a Query**
- **Learning MySQL statements and Clauses**

## Typographical Conventions
In MySQL, you can often troubleshoot your own errors, by highlighting over red_underlined text as can be seen in the example below.

    SELECT *
    FROM Reef
    WHERE reefName IN <span style="text-decoration: underline">SELECT</span> // (1)
    
    1."SELECT is not valid at this position for this server version, expecting FOR, LOCK, TABLE, VALUES, WITH, '('
    
Statements and Clauses, and various datatypes such as strings in MySQL will often be highlighted in another color:

    SELECT u.id FROM user u, user grace
    WHERE grace.fName = "grace" AND grace.lname = "Jeon" AND(
    SELECT count(*) FROM (
    
## Notes and Warning Messages
> ⚠️: **EMOJI ZONE**: Dangerous action
> 📝: **EMOJI ZONE**: Additional information
