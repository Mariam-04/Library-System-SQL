# 📚 Library Management System – SQL Schema and Procedures
This project implements a **Library Management System** using SQL. It defines a relational database schema to manage books, authors, staff, readers, discussion rooms, book issuance, and recommendations. Additionally, it includes various stored procedures and triggers to automate core functionalities like issuing books, searching, and generating recommendations.

## 📁 Database Structure

The system includes the following tables:

- **`author`**: Stores author details.
- **`book`**: Contains book information including genre, rating, and availability.
- **`staff`**: Holds librarian and assistant librarian records.
- **`stafflogin`**: Manages staff authentication.
- **`readers`**: Stores library members' information.
- **`discussion_room`**: Represents rooms available for booking.
- **`room_bookings`**: Tracks booking of discussion rooms.
- **`issued_books`**: Records book issuance, return dates, and due dates.

## 🔁 Triggers

- **`CheckBookAvailability`**: Ensures a book is only issued if available.
- **`UpdateBookStatusAfterIssuing`**: Automatically updates book status post-issuance.

## 🔍 Stored Procedures

- `SearchBooksByAuthor` – Search books by author name.
- `SearchBooksByGenre` – Retrieve books by genre.
- `RecommendBooksByAgeAndGenre` – Recommend books based on reader age group and genre.
- `GetTopBestSellers` – Lists top 5 most issued books.
- `GetTopTrendingBooks` – Lists top-rated and frequently issued books.
- `DisplayBookSeries` – Lists books in a specific series.
- `DisplayLibrarianQualifications` – Shows librarian qualifications.

## 🧪 Sample Data

Sample records have been inserted into:

- **`author`**
- **`book`** (includes a Harry Potter series)
- **`readers`**
- **`issued_books`**
- **`staff`**

## ✅ How to Use

1. **Run the script** in your SQL environment (e.g., SQL Server Management Studio or Azure Data Studio).
2. Use the `EXEC` command to invoke stored procedures.
3. Modify or extend stored procedures as needed for additional functionality.

## 💡 Future Enhancements

- Add fine calculation for overdue books.
- Implement user roles and privileges.
- Create a front-end interface connected via APIs.
