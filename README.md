# Quora Posts Backend

A Quora-style posts application built from scratch while learning backend development with Node.js and Express.js.

The application allows users to create, view, edit, and delete posts through RESTful routes.

## Features

- Create a new post
- View all posts
- View an individual post
- Edit an existing post
- Delete a post
- Generate unique post IDs using UUID
- Method overriding for PATCH and DELETE requests
- Server-side rendering using EJS

## Tech Stack

- Node.js
- Express.js
- EJS
- JavaScript
- UUID
- Method Override

## RESTful Routes

| Method | Route | Purpose |
|--------|-------|---------|
| GET | `/posts` | View all posts |
| GET | `/posts/new` | Show create-post form |
| POST | `/posts` | Create a new post |
| GET | `/posts/:id` | View a specific post |
| GET | `/posts/:id/edit` | Show edit form |
| PATCH | `/posts/:id` | Update a post |
| DELETE | `/posts/:id` | Delete a post |

## Project Structure

```text
Quora-Posts-backend/
├── public/
│   └── style.css
├── views/
│   ├── index.ejs
│   ├── new.ejs
│   ├── show.ejs
│   └── edit.ejs
├── index.js
├── package.json
├── package-lock.json
├── .gitignore
└── README.md
```

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/vinaysharma-pgr/Quora-Posts-backend.git
```

### 2. Navigate to the project directory

```bash
cd Quora-Posts-backend
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the server

```bash
node index.js
```

### 5. Open the application

Visit:

```text
http://localhost:8080/posts
```

## What I Learned

This project was built as a hands-on backend learning project to understand:

- Express.js application setup
- Routing and HTTP methods
- Middleware
- Handling HTML form data
- RESTful route design
- CRUD operations
- Dynamic route parameters
- EJS templating
- Method overriding
- UUID-based resource identification
- Git and GitHub workflow

## Current Limitations

- Data is stored in memory and is lost when the server restarts.
- No database is currently used.
- No authentication or authorization is implemented.
- Input validation is minimal.

## Future Improvements

- Replace in-memory storage with MongoDB
- Use Mongoose for database operations
- Build JSON-based REST API endpoints
- Add input validation
- Add proper error handling
- Add user authentication and authorization