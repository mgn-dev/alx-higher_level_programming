# ALX Higher Level Programming

A project covering Python fundamentals through SQL, object-relational mapping, HTTP networking, and JavaScript web development.

## Overview

This project includes 22 tasks that build higher-level programming skills on top of a C foundation. The first half establishes Python syntax, control flow, data structures, object-oriented design, and test-driven development. The middle section introduces relational databases with raw SQL and SQLAlchemy ORM. The final task folders shift to HTTP clients, shell scripting for web requests, and JavaScript for scripting, DOM manipulation, web scraping, and jQuery.

Each task folder is a self-contained directory of numbered tasks (`0-`, `1-`, …) with checker-compatible entry points. Tasks increase in complexity—from single-file scripts to multi-class packages with unit tests and database-backed applications.

## Skills covered


- Write idiomatic Python using functions, classes, inheritance, and exception handling
- Work with lists, tuples, sets, and dictionaries for data modeling and transformation
- Apply test-driven development with `doctest` and `unittest`
- Design object hierarchies with encapsulation, property decorators, and class/instance attribute semantics
- Perform CRUD operations in MySQL using SQL and Python DB-API connectors
- Map Python classes to database tables with SQLAlchemy ORM and model relationships
- Send HTTP requests, parse responses, and interact with REST APIs from Python and the shell
- Write JavaScript for scripting, closures, prototypes, Node.js HTTP clients, and browser-side jQuery

## Tech Stack

| Category | Technologies |
|----------|-------------|
| Languages | Python 3, JavaScript (ES6), Bash, SQL |
| Databases | MySQL, SQLAlchemy ORM |
| Web | `urllib`, `requests`, cURL, Node.js HTTP, jQuery |
| Testing | `doctest`, `unittest` |
| Runtime | Ubuntu 20.04+, Node.js (JavaScript modules) |

## Project Structure

| Module | Directory | Focus |
|--------|-----------|-------|
| 0x00 | `0x00-python-hello_world` | Python syntax, printing, string formatting |
| 0x01 | `0x01-python-if_else_loops_functions` | Conditionals, loops, functions, FizzBuzz |
| 0x02 | `0x02-python-import_modules` | Imports, `sys.argv`, custom modules |
| 0x03 | `0x03-python-data_structures` | Lists, tuples, matrix operations |
| 0x04 | `0x04-python-more_data_structures` | Sets, dictionaries, comprehensions |
| 0x05 | `0x05-python-exceptions` | Try/except, safe type conversion |
| 0x06 | `0x06-python-classes` | Classes, methods, singly linked lists |
| 0x07 | `0x07-python-test_driven_development` | Doctests, edge-case validation |
| 0x08 | `0x08-python-more_classes` | Properties, area/perimeter geometry classes |
| 0x09 | `0x09-python-everything_is_object` | Object identity, mutability, `__slots__` |
| 0x0A | `0x0A-python-inheritance` | Subclassing, method overrides, MRO |
| 0x0B | `0x0B-python-input_output` | File I/O, JSON serialization |
| 0x0C | `0x0C-python-almost_a_circle` | OOP package: Base, Rectangle, Square |
| 0x0D | `0x0D-SQL_introduction` | MySQL DDL/DML, databases and tables |
| 0x0E | `0x0E-SQL_more_queries` | Joins, constraints, users, privileges |
| 0x0F | `0x0F-python-object_relational_mapping` | MySQLdb and SQLAlchemy models |
| 0x10 | `0x10-python-network_0` | cURL, Bash HTTP scripts, response parsing |
| 0x11 | `0x11-python-network_1` | `urllib`/`requests`, JSON APIs, GitHub API |
| 0x12 | `0x12-javascript-warm_up` | JS basics, loops, objects, arrow functions |
| 0x13 | `0x13-javascript_objects_scopes_closures` | Prototypes, closures, ES6 classes |
| 0x14 | `0x14-javascript-web_scraping` | Node.js HTTP, file I/O, Star Wars API |
| 0x15 | `0x15-javascript-web_jquery` | DOM selection, events, AJAX with jQuery |

## Key Implementations

- **Python OOP capstone (`0x0C`)** — A `models/` package with `Base`, `Rectangle`, and `Square` classes demonstrating inheritance, validation, and area/perimeter calculations
- **SQL foundations (`0x0D`–`0x0E`)** — Scripts for database creation, user management, joins across `states`/`cities`, and genre-based TV show queries
- **ORM integration (`0x0F`)** — Python scripts connecting to MySQL via `MySQLdb` and SQLAlchemy, including state/city relationship models and filtered queries
- **Network layer (`0x10`–`0x11`)** — Shell scripts for HTTP methods and status codes; Python clients for header inspection, POST payloads, JSON parsing, and GitHub commit history
- **JavaScript progression (`0x12`–`0x15`)** — From warm-up scripts through prototype-based rectangles, Star Wars API scraping, and interactive jQuery pages with dynamic DOM updates

## Getting Started

### Prerequisites

- Python 3.8+
- MySQL Server (modules `0x0D` onward)
- Node.js 14+ (modules `0x12` onward)
- `pycodestyle` (PEP 8 checks on Python tasks)

### Setup

```bash
git clone <repository-url>
cd alx-higher_level_programming
```

Install Python dependencies as needed per module (e.g., `MySQLdb`, `SQLAlchemy`, `requests`).

### Running Tasks

Python tasks are executed directly:

```bash
python3 0x00-python-hello_world/2-print.py
python3 0x0F-python-object_relational_mapping/0-select_states.py root password hbtn_0e_0_usa
```

JavaScript tasks use Node.js:

```bash
node 0x12-javascript-warm_up/0-javascript_is_amazing.js
node 0x14-javascript-web_scraping/100-starwars_characters.js
```

SQL scripts are applied against a local MySQL instance:

```bash
cat 0x0D-SQL_introduction/0-list_databases.sql | mysql -hlocalhost -uroot -p
```

Checker-style tests (where provided) use paired `main.py` files:

```bash
python3 0x06-python-classes/0-main.py
```

## Curriculum Context

This project is the second major programming segment in the ALX Software Engineering curriculum, following low-level C programming. It prepares learners for backend specialization work (`alx-backend`, `alx-backend-python`, `alx-backend-javascript`, `alx-backend-storage`, `alx-backend-user-data`) and the AirBnB clone project series. Mastery of Python OOP, SQL, and HTTP fundamentals here is prerequisite for Flask APIs, authentication systems, and full-stack web development later in the program.
