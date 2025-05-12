# 🔗 URL Shortener Microservice

The **URL Shortener Microservice** is an API that lets users shorten long URLs. It accepts a URL via POST request and returns a shortened version. When the user accesses the shortened URL, they are redirected to the original address.

## 📖 Learning Journey
This project was built while following [freeCodeCamp's Back End Development and APIs Course](https://www.freecodecamp.org/learn/back-end-development-and-apis).

## 🛠️ Tech Stack
- **Frontend:** HTML, CSS
- **Backend:** Node.js (Express.js)
- **Database:** MongoDB

## 🎯 Features
- Accepts a `POST` request to `/api/shorturl` with a `url` parameter.
- Returns a JSON response with:
  - `original_url`: The original URL provided by the user.
  - `short_url`: A unique numeric identifier for the shortened link.
- Redirects users to the original URL when they visit `/api/shorturl/:short_url`.

## 🚀 Usage Examples

### Request: POST URL
POST /api/shorturl https://www.example.com
**Response:**
```json
{
  "original_url": "https://www.example.com",
  "short_url": 1
}
```

### Request: Accssing Shortened URL
GET /api/shorturl/1
Redirects to:
https://www.example.com


## 📦 Installation & Setup
1. **Clone the repository:**
  ```sh
git clone https://github.com/calvinbayaua/boilerplate-project-urlshortener.git
cd boilerplate-project-urlshortener
  ```
2. **Install dependencies:**
  ```sh
  npm i
  ```
3. ** Create a .env file and add your MongoDB connection string:
  ```sh
  DB_URL:your_mongodb_connection_string
  ```
4. **Start the server**
  ```sh
  npm run start
  ```
