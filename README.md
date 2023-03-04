# TODO App

This TODO App is used as an app sample in learning kubernetes techs.

It supports the following API.

- `GET /todos`: Lists all todos
- `POST /todos`: Creates a new todo
- `PUT /todos/:id`: Updates the description of a todo
- `DELETE /todos/:id`: Deletes a todo

## Request body format

When calling `POST` or `PUT` methods, the request body should look like this:

```json
{
  "todo": {
    "description": "(todo description)"
  }
}
```

## UUIDs

For IDs, it uses "UUIDs" (Universally Unique IDs). They can be generated using the `uuid` package, and are guaranteed never to be the same.
