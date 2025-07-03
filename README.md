# Library Management System 📚

A comprehensive Java Swing-based desktop application for managing library operations including book management, staff management, and user authentication.

## 🚀 Features

### 📖 Book Management
- **Add Books**: Add new books to the library database with details like Book ID, Name, Author, Publisher, and Quantity
- **View Available Books**: Display all books currently available in the library
- **Update Books**: Modify existing book information
- **Remove Books**: Delete books from the library database

### 👥 Staff Management
- **Add Staff**: Register new library staff members
- **View Staff Details**: Display all staff information
- **Update Staff**: Modify existing staff information
- **Remove Staff**: Delete staff records from the database

### 🔐 Authentication
- **Secure Login**: Admin login system with username and password authentication
- **Dashboard**: Central hub for accessing all library management features

## 🛠️ Technology Stack

- **Language**: Java (Swing GUI Framework)
- **Database**: MySQL
- **IDE**: NetBeans
- **Build Tool**: Apache Ant (build.xml)

## 📁 Project Structure

```
Library Management System/
├── src/                          # Source code files
│   ├── LoginPage.java           # Authentication page
│   ├── DashBoard.java           # Main dashboard
│   ├── Add_Books.java           # Add new books
│   ├── Books_Available.java     # View all books
│   ├── Update_Books.java        # Update book information
│   ├── Remove_Books.java        # Remove books
│   ├── Add_Staff.java           # Add new staff
│   ├── Staff_Details.java       # View staff details
│   ├── Update_Staff.java        # Update staff information
│   ├── Remove_Staff.java        # Remove staff
│   └── *.form files             # NetBeans GUI form files
├── build/                       # Compiled classes
├── nbproject/                   # NetBeans project files
├── test/                        # Test files
├── build.xml                    # Ant build configuration
└── manifest.mf                  # Manifest file
```

## 🗄️ Database Schema

The application uses MySQL database with the following tables:

### Books Table
- `BOOK_ID` - Unique identifier for books
- `BOOK_NAME` - Name of the book
- `AUTHOR` - Author of the book
- `PUBLISHER` - Publisher information
- `QUANTITY` - Number of copies available

### Staff Table
- Staff ID
- Staff Name
- Additional staff information

### Admin Table
- `USER_ID` - Admin username
- `PASSWORD` - Admin password

## ⚙️ Setup and Installation

### Prerequisites
- Java Development Kit (JDK) 8 or higher
- MySQL Server
- NetBeans IDE (recommended)

### Database Setup
1. Install and start MySQL server
2. Create a new database for the library management system
3. Create the required tables (`books`, `staff`, `admin`)
4. Update database connection parameters in the Java files:
   ```java
   String url = "jdbc:mysql://localhost:3306/your_database_name";
   String user = "your_mysql_username";
   String pwd = "your_mysql_password";
   ```

### Application Setup
1. Clone or download the project
2. Open the project in NetBeans IDE
3. Ensure MySQL Connector/J is added to the project libraries
4. Build the project using NetBeans or run:
   ```bash
   ant compile
   ```
5. Run the application:
   ```bash
   ant run
   ```

## 🎯 Usage

1. **Login**: Start the application and enter admin credentials
2. **Dashboard**: Access the main dashboard with all available options
3. **Book Operations**:
   - Click "BOOKS AVAILABLE" to view all books
   - Click "ADD BOOKS" to add new books
   - Use "UPDATE BOOKS" to modify existing book information
   - Use "REMOVE BOOKS" to delete books
4. **Staff Operations**:
   - Click "STAFF DETAILS" to view all staff
   - Click "ADD STAFF" to register new staff
   - Use update and remove options for staff management

## 🎨 User Interface

The application features a clean and intuitive GUI built with Java Swing:
- **Color Scheme**: Professional blue and teal color palette
- **Fonts**: Segoe UI for modern appearance
- **Layout**: Centered windows with consistent positioning
- **Navigation**: Easy-to-use button-based navigation

## 👨‍💻 Author

**Vamshi R A**

## 🔧 Build Information

- **Project Name**: Library_Management_System
- **Build Tool**: Apache Ant
- **IDE**: NetBeans
- **Main Class**: LoginPage (Entry point)

## 📝 Notes

- The application uses NetBeans GUI Builder for form design
- Database connection parameters need to be configured before running
- All forms are designed to be disposed on close to prevent memory leaks
- The application includes proper error handling and user feedback

## 🚀 Future Enhancements

- [ ] Add book borrowing and return functionality
- [ ] Implement member management system
- [ ] Add reporting and analytics features
- [ ] Include book search and filter options
- [ ] Add email notifications for due dates
- [ ] Implement backup and restore functionality

---

*This project demonstrates the implementation of a complete CRUD (Create, Read, Update, Delete) application using Java Swing and MySQL database connectivity.*