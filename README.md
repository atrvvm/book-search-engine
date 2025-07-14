# 📚 Book Search Engine

A full-stack application that allows users to search for books using the Google Books API and save their favorite titles. Originally built using the MERN stack with a RESTful API, the backend has been refactored to use **GraphQL with Apollo Server**. The front end is powered by **React**, and user authentication is handled via **JWT**.

> 🔗 **Live Demo**: [Deployed App on Render](#)

---

## 🚀 Features

- Search for books via Google Books API
- User authentication with JWT and Apollo
- Save and manage your favorite books
- Fully refactored backend using Apollo Server and GraphQL
- Deployed using Render and MongoDB Atlas

---

## ✅ Acceptance Criteria

- View search results with book title, author, description, image, and external link
- Sign up and log in through a modal
- Authenticated users can save and delete books from their personal collection
- UI updates dynamically based on user authentication status

---

## ⚙️ Technologies Used

- **Frontend**: React, Apollo Client, GraphQL, Bootstrap
- **Backend**: Node.js, Express.js, MongoDB, Mongoose, Apollo Server
- **Authentication**: JWT
- **Deployment**: Render (App) + MongoDB Atlas (Database)

---

## 🧩 GraphQL Schema Overview

### Types

- **User**
  - `_id`, `username`, `email`, `bookCount`, `savedBooks`
- **Book**
  - `bookId`, `authors`, `description`, `title`, `image`, `link`
- **Auth**
  - `token`, `user`

### Queries

```graphql
me: User
