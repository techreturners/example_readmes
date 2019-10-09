# Todo Application - Backend

This is the back end API of a Todo Application, built throughout the [Tech Returners](https://techreturners.com) Your Journey Into Tech course. It is consumed by a front end React application, available [here](https://github.com/your-backend-repo) and connects to an RDS Database.

The hosted version of the application is available here: [https://github.com/whatever-link-here](https://github.com/whatever-link-here).

### Technology Used

This project uses the following technology:

- Serverless Framework
- JavaScript (ES2015+)
- Express
- SQL
- Mysql library
- AWS Lambda and API Gateway
- AWS RDS
- ESLint

### Endpoints

The API exposes the following endpoints:

---

##### GET /tasks

[https://0jjep9sqze.execute-api.eu-west-1.amazonaws.com/dev/tasks](https://0jjep9sqze.execute-api.eu-west-1.amazonaws.com/dev/tasks)

Responds with JSON containing all tasks in the Database.

---

##### POST /tasks

[https://0jjep9sqze.execute-api.eu-west-1.amazonaws.com/dev/tasks](https://0jjep9sqze.execute-api.eu-west-1.amazonaws.com/dev/tasks)

Will create a new task when sent a JSON payload in the format:

```json
{
  "text": "walk dog",
  "completed": false,
  "date": "2019-12-17"
}
```

---

##### DELETE /tasks/:taskId

[https://0jjep9sqze.execute-api.eu-west-1.amazonaws.com/dev/tasks/:taskId](https://0jjep9sqze.execute-api.eu-west-1.amazonaws.com/dev/tasks/:taskId)

Deletes the task of the given ID.

---

##### PUT /tasks/:taskId

[https://0jjep9sqze.execute-api.eu-west-1.amazonaws.com/dev/tasks/:taskId](https://0jjep9sqze.execute-api.eu-west-1.amazonaws.com/dev/tasks/:taskId)

Will update a task when sent a JSON payload in the format:

```json
{
  "text": "walk dog",
  "completed": true,
  "date": "2019-12-17"
}
```
