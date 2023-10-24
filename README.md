# DarkGPT API for Node.js

This repository contains a simple and modern API for interacting with ChatGPT-Dark using Node.js. It's fast, free, and easy to use.

## Getting Started

First, clone the repository:

```bash
git clone https://github.com/ReactMVC/DarkGPT-API.git
```

Navigate into the project directory:

```bash
cd DarkGPT-API
```

Install the necessary dependencies:

```bash
npm install
```

Start the server:

```bash
node index.js
```
The server will start running on port 3000.

## Usage

The API provides two endpoints, both of which accept a `text` parameter:

- GET `/`
- POST `/`

## Fetch

##### GET

```javascript
fetch('http://localhost:3000/?text=Hello', {
  method: 'GET',
})
.then(response => response.json())
.then(data => console.log(data));
```

##### POST

```javascript
fetch('http://localhost:3000/', {
  method: 'POST',
  headers: {
    'Content-Type': 'application/json; charset=utf-8',
  },
  body: JSON.stringify({ text: 'Hello' }),
})
.then(response => response.json())
.then(data => console.log(data));
```

## Axios

##### GET

```javascript
axios.get('http://localhost:3000/', {
  params: {
    text: 'Hello',
  },
})
.then(response => console.log(response.data));
```

##### POST

```javascript
axios.post('http://localhost:3000/', {
  text: 'Hello',
}, {
  headers: {
    'Content-Type': 'application/json; charset=utf-8',
  },
})
.then(response => console.log(response.data));
```

## Contact

For any issues, suggestions, or general feedback, please contact:

- Name: Hossein Pira
- Email: h3dev.pira@gmail.com
- Telegram: [@h3dev](https://t.me/h3dev)

Enjoy using the ChatGPT-Dark API!