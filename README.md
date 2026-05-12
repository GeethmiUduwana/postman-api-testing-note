# Postman Notes

## Introduction to Postman

Postman is a popular API testing and development tool used by developers to design, test, debug, and document APIs easily.

It provides a graphical user interface (GUI) to send HTTP requests and receive responses without writing complex code.

---
# Features of Postman

## 1. API Testing

- Send requests to APIs
- Check API responses
- Validate status codes and data

## 2. User-Friendly Interface

- Easy GUI
- No need to use command line tools

## 3. Supports Multiple HTTP Methods

- GET
- POST
- PUT
- DELETE
- PATCH
## 4. Collections

- Save API requests in groups
- Reuse requests easily

## 5. Environment Variables

- Store values like:
  - URLs
  - Tokens
  - Usernames
  - Passwords

## 6. Automation Testing

- Write test scripts using JavaScript
- Automate API validation

## 7. API Documentation

- Generate and share API documentation

## 8. Collaboration

- Team members can share collections and environments

---
2. Download the application
3. Install it on:
   - Windows
   - Linux
   - macOS

---

# Installation of Postman

1. Visit the official website:

[Postman Official Website](https://www.postman.com/)

# HTTP Methods in Postman

| Method | Purpose |
|---|---|
| GET | Retrieve data |
| POST | Send new data |
| PUT | Update existing data |
| DELETE | Remove data |
| PATCH | Partially update data |

---
# Components of Postman Interface

## 1. Request Section

Used to:
- Enter API URL
- Select HTTP method
- Add headers and body

## 2. Response Section

Displays:
- Status code
- Response body
- Headers
- Response time

## 3. Collections

Stores saved requests.

## 4. Environment

Stores variables for different systems.

---

# Creating a GET Request

## Steps

1. Open Postman
2. Select **GET**
3. Enter API URL
4. Click **Send**
5. View the response
### Example API

```bash
https://jsonplaceholder.typicode.com/posts
```

---

# Creating a POST Request

## Steps

1. Select **POST**
2. Enter API URL
3. Go to **Body**
4. Select **raw → JSON**
5. Enter JSON data
6. Click **Send**

### Example JSON

```json
{
  "title": "Test Post",
  "body": "Hello World",
  "userId": 1
}
```

---

# Status Codes

| Code | Meaning |
|---|---|
| 200 | OK |
| 201 | Created |
| 400 | Bad Request |
| 401 | Unauthorized |
| 404 | Not Found |
| 500 | Internal Server Error |

---
# Headers in Postman

Headers provide additional information about the request.

### Example

```bash
Content-Type: application/json
Authorization: Bearer token
```

---

# Authorization Types

| Type | Description |
|---|---|
| Basic Auth | Username and password |
| Bearer Token | Token-based authentication |
| API Key | Unique access key |
| OAuth 2.0 | Secure authentication framework |

---

# Environment Variables

Environment variables help avoid repeating values.

### Example

| Variable | Value |
|---|---|
| base_url | https://api.example.com |
| token | abc123 |

Usage:

```bash
{{base_url}}/users
```

---

# Writing Tests in Postman

Postman supports JavaScript for testing.

### Example Test Script

```javascript
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```

---
# Collections in Postman

Collections are used to:
- Organize requests
- Share APIs
- Run automated tests

Benefits:
- Easy maintenance
- Reusability
- Team collaboration

---

# Advantages of Postman

- Easy to use
- Supports automation
- Fast API testing
- Good collaboration features
- Supports multiple environments
- Helps in debugging APIs

---

# Limitations of Postman

- Large collections may become slow
- Requires internet for some cloud features
- Advanced automation may require coding knowledge

---

# Common Uses of Postman

- API development
- API testing
- Backend debugging
- Automation testing
- API documentation
- Team collaboration

---
# Conclusion

Postman is one of the most widely used API testing tools in software development. It simplifies API creation, testing, debugging, and documentation with an easy-to-use graphical interface. It is highly useful for developers, testers, and DevOps engineers.
