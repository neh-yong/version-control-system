# Notes

## 1. Version Control System (VCS)

A **Version Control System (VCS)** is a tool that records changes made to files over time. It allows developers to track modifications, collaborate with others, and restore previous versions if needed.

### Benefits

* Tracks the history of changes.
* Makes collaboration easier.
* Allows reverting to previous versions.
* Helps resolve conflicts when multiple developers work on the same project.

---

## 2. Git

**Git** is a **distributed Version Control System (VCS)** created by **Linus Torvalds** in 2005. It runs on your local machine and helps you track changes to your project's files.

### Key Features

* Tracks file changes.
* Creates snapshots using commits.
* Supports branching and merging.
* Works offline.
* Fast and lightweight.

**Example Commands**

```bash
git init
git add .
git commit -m "Initial commit"
```

---

## 3. GitHub

**GitHub** is a cloud-based platform that hosts Git repositories. It provides collaboration features on top of Git, allowing developers to store, share, and work together on projects.

### Key Features

* Remote repository hosting.
* Team collaboration.
* Pull Requests.
* Issue tracking.
* Code reviews.
* GitHub Actions (CI/CD).

---

## 4. Git vs GitHub

| Git                                   | GitHub                                             |
| ------------------------------------- | -------------------------------------------------- |
| A Version Control System.             | A cloud platform for hosting Git repositories.     |
| Installed on your computer.           | Accessible through a web browser.                  |
| Tracks changes locally.               | Stores repositories remotely.                      |
| Works without an internet connection. | Requires an internet connection for most features. |
| Used for version control.             | Used for collaboration and repository hosting.     |

## 5. Common Project Folders (Node.js + Express)

### `controllers/`

Contains the **business logic** of the application. Controllers receive requests from routes, process the request, interact with models, and send responses back to the client.

**Examples**

* `authController.js`
* `userController.js`
* `repositoryController.js`
* `issueController.js`

---

### `routes/`

Defines the application's API routes. Each route maps an HTTP request to a controller function.

**Examples**

* Authentication routes
* User routes
* Repository routes
* Issue routes

---

### `models/`

Contains the database schemas and models. Models define the structure of the data and provide methods to interact with the database.

**Examples**

* `User.js`
* `Repository.js`
* `Issue.js`

---

### `config/`

Stores configuration files and external service setups used throughout the application.

**Examples**

* Database connection (`db.js`)
* Authentication configuration
* Cloud storage configuration
* Environment configuration

---

### `middleware/`

Contains middleware functions that execute before the request reaches the controller.

**Common Uses**

* Authentication
* Authorization
* Request validation
* Error handling
* Logging

---

### `services/`

Contains reusable business logic that can be shared across multiple controllers.

**Examples**

* Email service
* File upload service
* Notification service
* Payment service

---

### `utils/`

Contains helper or utility functions used across the project.

**Examples**

* Password hashing
* Token generation
* Date formatting
* Common helper functions

---

### `validators/`

Contains request validation logic to ensure incoming data is valid before processing.

**Examples**

* Login validation
* Registration validation
* Repository validation

---

### `public/`

Stores static files that are directly served to users.

**Examples**

* Images
* CSS files
* JavaScript files
* Fonts

---

### `views/`

Contains server-side templates (used with template engines like EJS, Pug, or Handlebars).

---

### `uploads/`

Stores files uploaded by users.

**Examples**

* Profile pictures
* Documents
* Repository assets

---

### `tests/`

Contains automated tests for the application.

**Examples**

* Unit tests
* Integration tests
* API tests

---

### Root Files

#### `server.js` / `app.js`

The application's entry point. Initializes the server, middleware, routes, and configurations.

#### `package.json`

Stores project metadata, dependencies, scripts, and other project configurations.

#### `.env`

Stores environment variables such as database URLs, API keys, and secret keys. This file should **never** be committed to GitHub.

#### `.gitignore`

Specifies which files and folders Git should ignore (e.g., `node_modules/`, `.env`).
