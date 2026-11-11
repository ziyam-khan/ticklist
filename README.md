<h1 align="center">ticklist</h1>
<p align="center">A small task tracker: tasks with a day, a reminder you toggle with a double click, and a list that lives in MongoDB.</p>

<p align="center">
  <img alt="React" src="https://img.shields.io/badge/ui-React%2018-61dafb">
  <img alt="Express" src="https://img.shields.io/badge/api-Express-444">
  <img alt="MongoDB" src="https://img.shields.io/badge/db-MongoDB-47a248">
</p>

## What it does

- Add a task with its day and time, and whether it needs a reminder.
- Double-click a task to switch its reminder on or off; reminded tasks are marked in the list.
- Delete a task when it is done. An About page sits on its own route.

Built in May 2023 as a final assignment.

## Stack

| Part | Tools |
|---|---|
| Interface | React 18, React Router 6, React Icons |
| API | Node.js, Express, Mongoose |
| Database | MongoDB (local, `ticklist`) |

## Run it

Start MongoDB on `localhost:27017`, then in two terminals:

```sh
cd backend && npm install && node index.js     # API on :5000
cd frontend && npm install && npm start        # interface on :3000
```

## API

| Method | Path | Does |
|---|---|---|
| `GET` | `/tasks` | Every task |
| `POST` | `/task` | Add one: `{ id, text, day, reminder }` |
| `DELETE` | `/task/:id` | Remove one |

---

By [Ziyam Khan](https://ziyamkhan.com) · [GitHub](https://github.com/ziyam-khan)
