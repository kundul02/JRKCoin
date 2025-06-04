# JRK Coin

JRK Coin is a demo cryptocurrency website showcasing a fictional digital currency. The project is a static HTML page styled with Tailwind CSS (loaded via CDN) and includes a small tool that can fetch explanations for crypto related terms using Google's Gemini API.

## Viewing the Site

Open `index.html` in any modern browser. No build step is required because all dependencies are loaded through CDNs.

## Gemini API Key Configuration

The explanatory tool in `index.html` requires a Gemini API key. Edit the line defining `apiKey` near the bottom of the file:

```javascript
const apiKey = "YOUR_GEMINI_API_KEY";
```

Replace the placeholder value with your own key. Once set, the "Explain a Crypto Term" section on the page will send requests to the Gemini API when you click **Explain**.

## Dependencies

- [Tailwind CSS](https://tailwindcss.com) via CDN
- Google Fonts (Inter) and Material Icons via CDN

Because everything is fetched from CDNs, there are no additional installation steps.

## Deployment

JRK Coin is a purely static site. You can deploy it to any static hosting provider (for example GitHub Pages or a basic web server) by uploading `index.html` and the `Site` file. Alternatively, you can serve the repository locally with any simple HTTP server if you prefer not to open the file directly.

