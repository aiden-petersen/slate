---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - json

includes:
  - errors

search: true
---

# Introduction

Welcome to the TaskTracker API! This API is part of the [TaskTracker](https://github.com/aiden-petersen/TaskTracker) personal project. This webpage describes the API and demonstates usage.

The API can be used to retrieve, create and update tasks. Current features include: Tracking tasks and time spend on each task.

# Tasks

## Get All Tasks

> The request returns JSON structured like this:

```json
  {
  }
```

This endpoint retrieves all completed tasks. Sorted by date and grouped by the day they were started.

### HTTP Request

`GET http://localhost:3003/api/tasks`

## Get a Task


> The above command returns JSON structured like this:

```json
{
}
```

This endpoint gets a specific task.

### HTTP Request

`GET http://localhost:3003/api/tasks/<task_id>`

### URL Parameters

Parameter | Description
--------- | -----------
task_id | The ID of the task

## Create a Task

> The above command returns JSON structured like this:

```json
{
}
```

This endpoint creates a new task.

### HTTP Request

`POST http://localhost:3003/api/tasks/`

### Form Parameters

Parameter | Description
--------- | -----------
title | The title for the given task
start_date | The start date for the given task
stop_date | The stop date for the given task

## Delete a Task


> The above command returns JSON structured like this:

```json
{

}
```

This endpoint deletes a specific task.

### HTTP Request

`DELETE http://localhost:3003/api/tasks/<task_id>`

### URL Parameters

Parameter | Description
--------- | -----------
task_id | The ID of the task to delete

