# Theus Chatbot Embed

This repository contains the frontend code for the Theus chatbot UI. It's designed to be hosted using GitHub Pages and embedded into a Wix website via an HTML Embed (iFrame) element.

## Description

This is a self-contained `index.html` file that includes:
*   HTML structure (`<div id="root">`)
*   CSS styles within `<style>` tags
*   React component code (JSX) within `<script type="text/babel">` tags
*   CDN links to load external libraries:
    *   React (`react@17`)
    *   ReactDOM (`react-dom@17`)
    *   UUID (`uuid@8.3.2`)
    *   Babel Standalone (`@babel/standalone`) - for in-browser JSX transformation.
*   Connection logic to the backend API: `https://theusv3-gateway-740868556894.us-central1.run.app`

## Usage for Wix Embedding

1.  **Host:** Ensure this repository is hosted via GitHub Pages (Settings -> Pages).
2.  **Filename:** The main file must be named `index.html` for the base URL to work directly.
3.  **Embed:** In the Wix Editor:
    *   Add an "Embed Code" -> "Embed HTML" element.
    *   Set the embed type to "Website Address".
    *   Paste the GitHub Pages URL for this repository (e.g., `https://aigorahub.github.io/theus-chatbot-embed/`) into the address field.
    *   Resize the Wix HTML Embed element as needed.

## Development / Updating

*   To update the chatbot's appearance or functionality, edit the CSS or JavaScript sections within the `index.html` file directly.
*   Commit and push changes to the `main` branch of this repository.
*   GitHub Pages will automatically rebuild and deploy the updated `index.html` file (allow a minute or two for changes to reflect).