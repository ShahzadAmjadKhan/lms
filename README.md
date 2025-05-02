# Library Management System

A modern web-based Library Management System built with Spring Boot and Thymeleaf.

## Features

- **Book Management**
  - Add, edit, and delete books
  - Search books by title, author, or genre
  - Track book availability and quantity

- **Patron Management**
  - Add, edit, and delete patron information
  - Search patrons by name
  - Store contact and address details

- **Transaction Management**
  - Record book borrowings and returns
  - Track due dates and fines
  - Manage transaction status

## Tech Stack

- **Backend**
  - Spring Boot
  - Spring MVC
  - Thymeleaf
  - Lombok

- **Frontend**
  - Bootstrap 5
  - Bootstrap Icons
  - JavaScript

## Prerequisites

- Java 17 or higher
- Maven
- Your favorite IDE (IntelliJ IDEA, Eclipse, etc.)

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd lms
   ```

2. Build the project:
   ```bash
   mvn clean install
   ```

3. Run the application:
   ```bash
   mvn spring-boot:run
   ```

4. Access the application at `http://localhost:8080`

## API Documentation

The system provides RESTful APIs for managing books, patrons, and transactions. The API documentation is available in Swagger format:

### Books API
- `GET /lms/api/v1/books` - List all books
- `GET /lms/api/v1/book/{id}` - Get book by ID
- `POST /lms/api/v1/book` - Add new book
- `PUT /lms/api/v1/book/{id}` - Update book
- `DELETE /lms/api/v1/book/{id}` - Delete book

### Patrons API
- `GET /lms/api/v1/patrons` - List all patrons
- `GET /lms/api/v1/patron/{id}` - Get patron by ID
- `POST /lms/api/v1/patron` - Add new patron
- `PUT /lms/api/v1/patron/{id}` - Update patron
- `DELETE /lms/api/v1/patron/{id}` - Delete patron

### Transactions API
- `GET /lms/api/v1/transactions` - List all transactions
- `GET /lms/api/v1/transaction/{id}` - Get transaction by ID
- `POST /lms/api/v1/transaction` - Add new transaction
- `PUT /lms/api/v1/transaction/{id}` - Update transaction
- `DELETE /lms/api/v1/transaction/{id}` - Delete transaction

## Project Structure

```
src/
├── main/
│   ├── java/
│   │   └── com/
│   │       └── lms/
│   │           ├── features/        
│   │           ├── security/
│   │           ├── LmsApplication.java
│   │           └── AppConfiguration.java
│   └── resources/
│       ├── static/                 # Static assets
│       ├── templates/              # Thymeleaf templates
│       └── application.properties  # Configuration
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 