[![VS Code Marketplace](https://img.shields.io/visual-studio-marketplace/v/Payamaya.node-express-snippets)](https://marketplace.visualstudio.com/items?itemName=Payamaya.node-express-snippets)
[![Installs](https://img.shields.io/visual-studio-marketplace/i/Payamaya.node-express-snippets)](https://marketplace.visualstudio.com/items?itemName=Payamaya.node-express-snippets)
[![Rating](https://img.shields.io/visual-studio-marketplace/r/Payamaya.node-express-snippets)](https://marketplace.visualstudio.com/items?itemName=Payamaya.node-express-snippets)

# Node ExpressSnippet for VS Code

Essential Express.js snippets for faster Node.js development. Includes middleware, routing, error handling, and common API patterns to accelerate your Express application development workflow.

## Installation

### From VS Code:

1. Open VS Code
2. Press `Ctrl+Shift+X` to open Extensions
3. Search for **"Node ExpressSnippet"**
4. Click **Install**

### From Marketplace:

Visit: [Node ExpressSnippet on VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=Payamaya.node-express-snippets)

## Features

- **Quick Express server setup** - Get started in seconds
- **Common route patterns** - GET, POST, PUT, DELETE routes
- **Middleware templates** - Custom middleware with error handling
- **Error handling** - Structured error responses
- **Security** - CORS, Helmet configurations
- **Best practices** - Follows Express.js conventions

## 🎥 Demo

![ExpressSnippet Demo](demo.gif)

### Quick Start:

1. Create a `.js` file
2. Type `express-server`
3. Press `Tab` to expand

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

## More Examples

### Express GET Route

```javascript
// Type: exp-get
app.get('/api/users', (req, res) => {
  try {
    // Your code here
    res.status(200).json({ success: true, data: result })
  } catch (error) {
    console.error('Error:', error)
    res.status(500).json({ success: false, error: error.message })
  }
})
```

### **4. Contributing Section**

```markdown
## Contributing

Found a bug or have a suggestion?

1. Open an issue on [GitHub](https://github.com/yourusername/node-express-snippets/issues)
2. Suggest new snippets
3. Report any problems

Want to add more snippets? Feel free to submit a PR!

## Support

If this extension helps you, consider:

- ⭐ Starring the repository
- 📝 Writing a review on the marketplace
- 🐛 Reporting issues
- 💡 Suggesting improvements

## Release Notes

See [CHANGELOG.md](CHANGELOG.md)

## License

MIT License
```
