# REST Todos API

## Description

This is a VERY simple REST API for a todo list. It is written in Go using `github.com/gin-gonic/gin` module.

## Usage

### Create a new todo

```bash
curl -X POST -H "Content-Type: application/json" -d '{"id": "6", "item": "Test todos", "completed": false}' http://localhost:8080/todos
```

### Get all todos

```bash
curl -X GET http://localhost:8080/todos
```

### Get a todo

```bash
curl -X GET http://localhost:8080/todos/1
```

### Toggle a todo

```bash
curl -X PATCH -H "Content-Type: application/json" http://localhost:8080/todos/1
```