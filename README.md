# Mini Library Management System 

## 📚 Course Information
**Module:** Object-Oriented Programming 1 (PROG211)  
**Semester:** August 2025 – January 2026  
**Lecturer:** Amandus Benjamin Coker  
**Assignment Type:** Individual (15%)  
**Title:** Mini Library Management System  
**Student Name:** [Your Full Name]  
**Student ID:** [Your Student ID]  
**Date of Submission:** [Insert Date]

---

## 🧭 Introduction
This Mini Library Management System is a **console-based application** written in **Python** to demonstrate the use of **lists, dictionaries, tuples, and functions** as core building blocks of programming.

The system does **not use Object-Oriented Programming (OOP)** concepts.  
Instead, it focuses on **functional programming** principles and **data structure manipulation**, fulfilling the PROG211 assignment requirements.

The program allows library staff and students to manage books, register members, borrow and return books, and view system data — all within a simple text-based interface.

---

## 🎯 Objectives
The objectives of this project are to:
1. Practice procedural programming using Python functions.
2. Demonstrate understanding of lists, dictionaries, and tuples.
3. Implement CRUD operations (Create, Read, Update, Delete).
4. Manage book borrowing and returning using logical checks.
5. Produce modular, readable, and well-documented code.
6. Validate system operations using simple `assert`-based tests.

---

## 🧩 System Features
### 📘 Book Management
- Add new books to the library.
- Update existing book details (title, author, genre, total copies).
- Delete books that are not currently borrowed.
- View all available books.
- Search books by title or author (case-insensitive).

### 👥 Member Management
- Add, update, or delete members.
- List all registered members.
- Track borrowed books per member.
- Prevent deletion of members with active borrowed books.

### 🔄 Borrowing and Returning
- Borrow a book if copies are available.
- Limit each member to **3 active borrowings**.
- Return books and automatically update total available copies.
- Display due dates for borrowed books (7-day period).
- Prevent borrowing if all copies are checked out.

### 🔐 Login System (Extra Feature)
The program includes a **login system** with role-based access:
| Role | Permissions |
|------|--------------|
| **Admin** | Manage books, members, and view borrow history |
| **Staff** | Borrow/return books and search catalog |
| **Student** | Borrow, return, and view personal borrow history |

---

## 🧱 Data Structures Used

### 1️⃣ Books – Dictionary
All books are stored in a **dictionary**, using the ISBN as the key and another dictionary as the value.

```python
books = {
    "B001": {"title": "Python Basics", "author": "Kevin Doe", "genre": "Non-Fiction", "total_copies": 3}
}
