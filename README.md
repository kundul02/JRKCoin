# JRKCoin

This project includes a static `index.html` page with JavaScript that calls the Gemini API. For security reasons, the API key is not stored in the repository. Instead, the code contains a placeholder value:

```javascript
const apiKey = "YOUR_API_KEY_HERE";
```

To run the site, supply your Gemini API key at runtime. A simple approach is to keep your key in a separate JavaScript file that is ignored by Git (for example, `config.js`) and load it before `index.html`'s script:

1. Create a file called `config.js` next to `index.html` and define your key:

```javascript
// config.js
const apiKey = "<your real API key>";
```

2. Add `config.js` to `.gitignore` so the key is never committed.
3. Include `config.js` in the page **before** the main script so that the variable is defined at runtime.

Alternatively, you can serve the key from a backend endpoint that reads the value from an environment variable and returns it to authenticated users. This keeps the key out of client-side code entirely.

Never commit your actual API key to the repository.
