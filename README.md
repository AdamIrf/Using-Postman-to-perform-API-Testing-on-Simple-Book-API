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

<img width="1267" height="630" alt="image" src="https://github.com/user-attachments/assets/bcb06726-fd08-47a9-b8c0-9e82f2120f84" />


| Metric | Value |
|--------|-------|
| **Total Requests** | 2,370 |
| **Requests/sec** | 13.31 |
| **Avg Response** | 704 ms |
| **Error Rate** | 0.00% |
| **Tests Passed** | 11/11 ✅ |

### Endpoint Results

<img width="1277" height="626" alt="image" src="https://github.com/user-attachments/assets/529d82de-2fe0-4b3a-bf68-587dab9dab74" />


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

<img width="1077" height="742" alt="image" src="https://github.com/user-attachments/assets/b71e0625-11ba-427b-b4dd-9ee529354504" />


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

<img width="1311" height="681" alt="image" src="https://github.com/user-attachments/assets/bf3db701-a495-4751-bfb9-8e1863bad8b9" />

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

**Status:** ✅ All Tests Passing | **Coverage:** 100%
