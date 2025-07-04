# 📚 Library Management System

A simple backend project to manage a library system using Node.js, Express.js, MongoDB (Mongoose), and TypeScript. This project includes full **CRUD operations for books**, a **borrow system** that updates inventory.

## 🚀 Key Features
✅ **CRUD for Books**: Create, Read, Update, and Delete operations for managing book entries  
✅ **Filter, SortBy, Sort, Limit**: Filter books by genre, sort in ascending or descending order by a specific field and limit the number of results returned

✅ **Borrowing System**: Borrow books and automatically update available stock  
✅ **Aggregation**: See how many copies of each book have been borrowed using Mongoose aggregation  
✅ **Inventory Control**: Automatically marks books unavailable when stock reaches zero  
✅ **Global Error Handling**: Centralized and structured error responses  



## 🛠 Tech Stack
- Node.js
- Express.js
- MongoDB (via Mongoose)
- TypeScript



## ⚙️ Installation

```
git clone https://github.com/Mohammadashif007/library-management
cd library-management
npm install

```


🔐 Environment Variables
Create a .env file in the root and add:

```
PORT=3000
DATABASE_URI=your_mongo_connection_string
```


## 🧪 Running the App

```
# Start development server
npm run start:dev

# OR build and run production
npm run build
node dist/server.js
```

📘 API Documentation

📚 Books API
Create a new book: `POST /api/books`
get all books: `GET /api/books`
get single book: `GET /api/books/:bookId`
update book: `PATCH /api/books/:bookId`
delete book: `DELETE /api/books/:bookId`

📙 Borrow API

Borrow one or more books. Automatically adjusts book stock and availability.
borrow books : `POST /api/borrow`
Return a summary of borrowed books : `GET /api/borrow`





