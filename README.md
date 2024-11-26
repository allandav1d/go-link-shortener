# GO LinkShortener

## Description

This is a simple link shortener that uses a REST API to shorten URLs. It is built using the Go programming language.
Project was created for learning purposes on the course Go by [Rocketseat](https://rocketseat.com.br/).

---

## 📋 Features

- **URL Shortening**: Easily convert long URLs into short, manageable codes.
- **Redirection**: Navigate to the original URL using the generated short code.
- **URL Validation**: Checks to ensure the provided URLs are valid before processing.
- **Lightweight Solution**: Relies on an in-memory map for URL storage, making it perfect for prototyping and educational purposes.
- **Scalable Design**: Designed to be extendable for future enhancements like database integration or advanced rate limiting.

---

## 🚀 How to Run the Project

### Prerequisites

- [Go](https://golang.org/) installed (version 1.23+ recommended).

### Steps

1. Clone the repository:

```bash
git clone https://github.com/allandav1d/go-link-shortener.git

cd go-link-shortener
```

2. Run the application:

```bash
go run .
```

---

## 🧪 Testing the Application

1. Use a tool like Postman or cURL to test the endpoints.

2. Example test with cURL:

• Create a short code:

```bash
  curl -X POST http://localhost:8080/shorten -d '{"url": "https://www.google.com"}' -H "Content-Type: application/json"
```

• Redirect:

```bash
curl -L http://localhost:8080/<short_code>
```

---

## ⚙️ Future Enhancements

- Database persistence (e.g., SQLite, PostgreSQL).
- Rate limiting to prevent abuse.
- Short code expiration.
- Web interface for easier usage.

## 📝 License

This project is licensed under the MIT License. See the LICENSE file for details.

Built with ❤️ and Go!
