# Using-Postman-to-perform-API-Testing-on-Simple-Book-API

## 📋 Overview

Postman API Testing collection for **Simple Book API** with complete CRUD operations.

---

## 🚀 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/status` | API health check |
| GET | `/books` | List all books |
| GET | `/books/{id}` | Get single book |
| POST | `/orders` | Place order |
| GET | `/orders` | Get all orders |
| GET | `/orders/{id}` | Get single order |
| PATCH | `/orders/{id}` | Update order |
| DELETE | `/orders/{id}` | Delete order |
| POST | `/clients` | Register client |

---

## 🔧 Environment Variables

| Variable | Value |
|----------|-------|
| `baseUrl` | `https://simple-books-api.click` |
| `accessToken` | `dbbfa4342f7ca699d70f5218e39...` |
| `orderId` | `ztnEcPbFnfa0xXfWzn7sr` |
| `bookId` | `5` |

---

## 📊 Test Results

### Run Summary

![Test Results](images/test-results.png)

| Metric | Value |
|--------|-------|
| **Total Requests** | 2,370 |
| **Requests/sec** | 13.31 |
| **Avg Response** | 704 ms |
| **Error Rate** | 0.00% |
| **Tests Passed** | 11/11 ✅ |

### Endpoint Results

![Endpoint Results](images/endpoint-results.png)

| Endpoint | Executed | Failed | Status |
|----------|----------|--------|--------|
| GET API Status | 2 | 0 | ✅ |
| GET List of books | 2 | 0 | ✅ |
| GET Get single book | 2 | 0 | ✅ |
| POST Order book | 1 | 0 | ✅ |
| GET All orders | 1 | 0 | ✅ |
| GET An order | 1 | 0 | ✅ |
| PATCH Update order | 1 | 0 | ✅ |
| DELETE Delete order | 1 | 0 | ✅ |

### Performance Dashboard

![Performance Dashboard](images/performance-dashboard.png)

| Metric | Value |
|--------|-------|
| **Test Duration** | 6.8s |
| **Avg Response** | 764 ms |
| **Min Response** | 283 ms |
| **Max Response** | 1803 ms |
| **Data Received** | 298.55 KB |

---

## 🛠️ Running Tests

### Postman
1. Import collection
2. Set environment variables
3. Run with Runner

### Newman (CLI)
```bash
npm install -g newman
newman run Simple-Book-API.postman_collection.json \
  -e Simple-Book-API.postman_environment.json
```

---

## ✅ Test Status

**All 11 assertions passing** ✨

![Newman Dashboard](images/newman-dashboard.png)

---

## 📁 Project Structure

```
📂 Simple-Book-API-Testing
├── 📄 Simple-Book-API.postman_collection.json
├── 📄 Simple-Book-API.postman_environment.json
├── 📂 images/
│   ├── test-results.png
│   ├── endpoint-results.png
│   ├── performance-dashboard.png
│   └── newman-dashboard.png
└── 📄 README.md
```

---

## 📝 Requirements

- [Postman](https://www.postman.com/)
- [Newman](https://learning.postman.com/docs/running-collections/using-newman-cli/) (optional)

---

## 📄 License

MIT License

---

**Status:** ✅ All Tests Passing | **Coverage:** 100%
