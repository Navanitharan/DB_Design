# Task Management Database

This repository contains SQL table models for managing users and their tasks.

## Tables

### Users
- `usr_id` (Primary Key): Unique identifier for each user.
- `usr_name`: Name of the user.
- `usr_email-id`: Email address of the user.
- `usr_password`: Password of the user.

### Task-Submitted
- `usr_id` (Foreign Key): References the `usr_id` in the Users table.
- `Task-Submitted`: Number of tasks submitted by the user.

### Task-link
- `usr_id` (Foreign Key): References the `usr_id` in the Users table.
- `task`: Task number.
- `frontend_link`: Link to the frontend code of the task.
- `backend_link`: Link to the backend code of the task.
- `submission_date`: Date when the task was submitted.
- `marks_allocated`: Marks allocated for the task submission.

## Normalization
All tables in this database follow the principles of normalization up to the Third Normal Form (3NF). 

- 1st Normal Form (1NF): All attributes contain atomic values, and there are no repeating groups.
- 2nd Normal Form (2NF): Non-prime attributes are fully functionally dependent on the primary key.
- 3rd Normal Form (3NF): There are no transitive dependencies.

## Usage
You can use these table models to set up a relational database management system (RDBMS) such as MySQL, PostgreSQL, or SQLite to manage users and their tasks efficiently.

## Contribution
Feel free to contribute to this repository by suggesting improvements or reporting issues.


