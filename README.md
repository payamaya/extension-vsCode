# ExpressSnippet for VS Code

Essential Express.js snippets for faster Node.js development. Includes middleware, routing, error handling, and common API patterns to accelerate your Express application development workflow.

## Features

- **Quick Express server setup** - Get started in seconds
- **Common route patterns** - GET, POST, PUT, DELETE routes
- **Middleware templates** - Custom middleware with error handling
- **Error handling** - Structured error responses
- **Security** - CORS, Helmet configurations
- **Best practices** - Follows Express.js conventions

## Snippets Included

| Prefix           | Description                    |
| ---------------- | ------------------------------ |
| `express-server` | Complete Express server setup  |
| `exp-get`        | GET route with error handling  |
| `exp-post`       | POST route with error handling |
| `exp-middleware` | Custom middleware function     |
| `exp-error`      | Error handling middleware      |
| `exp-params`     | Route with URL parameters      |
| `exp-static`     | Serve static files             |
| `exp-cors`       | CORS configuration             |
| `exp-helmet`     | Security headers with Helmet   |

## Usage

1. Type the snippet prefix (e.g., `express-server`)
2. Press `Tab` to expand
3. Fill in the placeholders using `Tab` to navigate

### Example

Type `express-server` and press `Tab`:

```javascript
const express = require('express')
const app = express()
const port = process.env.PORT || 3000

// Middleware
app.use(express.json())
app.use(express.urlencoded({ extended: true }))

// Routes
app.get('/', (req, res) => {
  res.send('Hello World!')
})

// Start server
app.listen(port, () => {
  console.log(`Server running on port ${port}`)
})
```
