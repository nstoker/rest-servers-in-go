# rest-servers-in-go

Following [Eli Bendersky's tutorial](https://eli.thegreenplace.net/2021/rest-servers-in-go-part-1-standard-library/)

## Local environment

The .env.example file contains sample settings.

```.env.example
SERVERPORT=4112             # The port the application is listening on
```

## Part 1: Using the Standard Library

See branch part_1 for the work in progress.

The API:

```text
POST   /task/              :  create a task, returns ID
GET    /task/<taskid>      :  returns a single task by ID
GET    /task/              :  returns all tasks
DELETE /task/<taskid>      :  delete a task by ID
GET    /tag/<tagname>      :  returns list of tasks with this tag
GET    /due/<yy>/<mm>/<dd> :  returns list of tasks due by this date
```
