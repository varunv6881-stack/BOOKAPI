# Book Management REST API

## Objective

Create a simple REST API using **Node.js** and **Express** to manage a list of books. The project performs CRUD (Create, Read, Update, Delete) operations without using a database. All book data is stored in memory.

## Tools Used

* Node.js
* Express.js
* VS Code
* Thunder Client / Postman

## Project Files

* `server.js`
* `package.json`
* `package-lock.json`
* `.gitignore`

## Installation

1. Clone or download the project.
2. Open the project folder in VS Code.
3. Install dependencies:

```bash
npm install
```

4. Start the server:

```bash
node server.js
```

The server will run at:

```
http://localhost:3000
```

## API Endpoints

### 1. Get All Books

* **Method:** GET
* **URL:** `/books`

### 2. Add a New Book

* **Method:** POST
* **URL:** `/books`

Example JSON:

```json
{
  "id": 3,
  "title": "C Programming",
  "author": "Dennis Ritchie"
}
```

### 3. Update a Book

* **Method:** PUT
* **URL:** `/books/:id`

Example:

```
PUT /books/3
```

Example JSON:

```json
{
  "title": "Advanced C",
  "author": "Dennis Ritchie"
}
```

### 4. Delete a Book

* **Method:** DELETE
* **URL:** `/books/:id`

Example:

```
DELETE /books/3
```

## Sample Initial Data

```json
[
  {
    "id": 1,
    "title": "Java",
    "author": "James"
  },
  {
    "id": 2,
    "title": "Python",
    "author": "Guido"
  }
]
```

## Features

* Create new books
* View all books
* Update existing books
* Delete books
* No database required
* Data stored in memory

## Author

Varun V
