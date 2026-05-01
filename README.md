# AI-Powered Content Generator

A lightweight browser-based app that uses the Google Gemini API to power a few quick content workflows:

- Ask any question
- Summarize pasted text
- Generate creative ideas
- Define terms with explanations

## Features

- Tab-based UI for switching between tools
- API key support through `config.js` or browser `localStorage`
- Loading and error states for API requests
- Auto-formatted numbered output for idea generation

## Project Files

- `index.html` - App markup and layout
- `styles.css` - Visual styling and responsive UI
- `app.js` - Main application logic and Gemini API calls
- `config.js` - API key configuration

## Setup

1. Open `config.js` and set your Gemini API key.
2. Open `index.html` in a browser, or serve the folder with a local static server.
3. Use the tabs to pick a feature and enter your prompt.

## Usage Notes

- The app uses the Gemini REST API from the browser.
- If no API key is available, the app will prompt for one and store it in `localStorage`.
- Keep your API key private and do not commit a production key to version control.

## Gemini API Key

You can create a key from Google AI Studio:

https://aistudio.google.com/app/apikey

## How It Works

The app loads `config.js` first, then `app.js`.

`app.js` validates the API key, sends prompts to Gemini, and renders the response in the active tab.
