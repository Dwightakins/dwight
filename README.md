# Dwight Calculator

Dwight Calculator is a real browser-based calculator with a plain-English math helper.

It lets you:

- type expressions like `12 + 8 / 4`
- use calculator buttons for common operations
- calculate percentages such as `150 * 15%`
- read a simple explanation of how the answer was produced
- review a short history of recent calculations

## What Is In This Project

- `docs/index.html` contains the full calculator app.
- `scripts/serve.js` starts a small local server for previewing the app in a browser.

## How To Run It Locally

From the project folder:

```powershell
node scripts/serve.js
```

Then open:

`http://127.0.0.1:4173/docs/`

## Supported Math

- addition: `4 + 5`
- subtraction: `9 - 3`
- multiplication: `7 * 6`
- division: `20 / 5`
- parentheses: `(18 - 6) * 3`
- decimals: `2.5 * 4`
- percent values: `150 * 15%`

## Plain-English Explanations

When you calculate something, the app:

1. reads the expression,
2. evaluates it in the correct order,
3. writes short step-by-step explanations in everyday language.

Example:

- `12 + 8 / 4`
- first it divides `8 / 4` to get `2`
- then it adds `12 + 2` to get `14`

## Deploying With GitHub Pages

Because the app is a static HTML file in `docs/index.html`, you can deploy it with GitHub Pages.

1. Push the repository to GitHub.
2. Open the repository settings.
3. Go to `Pages`.
4. Set the source to `Deploy from a branch`.
5. Choose `main` and the `/docs` folder.

GitHub Pages will then host the calculator site for you.
