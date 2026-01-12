# testgitdb

A test repository for demonstrating Git operations with database files.

## Database Schema

The `schema.sql` file contains a simple SQLite database schema with:
- `users` table: stores user information
- `posts` table: stores blog posts linked to users

## Usage

To create the database:
```bash
sqlite3 test.db < schema.sql
```

To view the data:
```bash
sqlite3 test.db "SELECT * FROM users;"
sqlite3 test.db "SELECT * FROM posts;"
```