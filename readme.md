# Exam Title:

## Implementing HTTP Methods in a Simple Project Structure

---

## Objective:

To practice creating and organizing files in a structured backend project and implement HTTP methods (GET, POST, PUT, DELETE) using `Node.js` and `Express`.

# Instructions:

Setup the Project:

- Create a new folder named `surname-semifinals`.
- Initialize the project with

```bash
npm init -y.
```

- Install `express` , `dotenv` for .env and `nodemon` using:

```bash
 npm i express dotenv nodemon
```

## Organize the Project:

Inside the folder, create the following structure:

```bash
surname-semifinals/
├── server.js
├── routes/
│   └── taskRoutes.js
├── controllers/
│   └── taskController.js
├── models/
│   └── Tasks.js
└── package.json
└── .env
└── .gitignore
```

Add some mock data in `.models/Tasks.js`, such as:

```javascript
// models/Task.js
let task = [
  { id: 1, task: "Learn HTTP Methods", status: "Incomplete" },
  { id: 2, task: "Organize Project Structure", status: "Complete" },
];

module.exports = items;
```

## Implement HTTP Methods with API Endpoints:

In `taskController.js`, implement the following logic:

- GET `/api/tasks` - Fetch all tasks.
- POST `/api/tasks` - Add a new task.
- PUT `/api/tasks/:id` - Update a specific task by id.
- DELETE `/api/tasks/:id` - Remove a specific task by id.

In `taskRoutes.js` (route file), create routes that map to the above API endpoints and link them to their corresponding controller methods.

In `server.js,` set up the Express app, import the route file, and configure middleware for JSON parsing.

Test the API:

- Use Postman or a similar tool to test each route:

```bash
http://localhost:3000
```

---

## Deliverables:

- The completed project folder.
- A short note explaining each HTTP method they implemented, the corresponding endpoint, and how they tested it.

## Submission:

- Submit the repo link and send it through Google Classroom.
- Send also your `Admission Slip` (no slip no grade)
