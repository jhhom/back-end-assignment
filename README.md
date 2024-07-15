# Back-end test assignment

Create a back-end API project for a to-do application in any programming language using any relational database you're comfortable using (e.g MySQL, PostgreSQL, SQLite).

The project needs to have 3 APIs:

1. GET /todos
2. POST /todos
3. DELETE /todos/:todo_id

## 1. API Requirements

### 1. GET /todos

Return an array of to-do objects

Sample response expected from a successful API call:

- `title` is the title of the to-do item
- `created_at` is the time the record is created in the database

```json
[
  {
    "id": 1,
    "title": "Buy groceries",
    "created_at": "2021-09-01T03:29:23.293182Z"
  },
  {
    "id": 2,
    "title": "Wash dishes",
    "created_at": "2021-09-01T03:29:23.293182Z"
  }
]
```

### 2. POST /todos

Sample request body:

Extra: Add a validation so that empty `title` is rejected

```json
{
  "title": "Buy groceries"
}
```

Sample response

```json
{
  "id": 3,
  "title": "Buy groceries",
  "created_at": "2021-09-01T03:29:23.293182Z"
}
```

### 3. DELETE /todos/:todo_id

Sample response

```json
{ "message": "Todo item deleted successfully" }
```

## 2. Submission

May upload the project to GitHub and provide us the GitHub repo link.
