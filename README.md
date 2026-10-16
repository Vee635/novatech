# NovaTech — Local functional website (Node + static)

This repository contains a demo static landing page with a simple Express backend to accept signups and store them locally in data/emails.json.

Files included:
- index.html
- styles.css
- script.js
- server.js (Express server)
- package.json
- .gitignore

Quick start (local):
1. Clone the repo or download the files.
2. In the project folder, install dependencies:
   npm install
3. Start the server:
   npm start
4. Open http://localhost:3000

API Endpoints:
- POST /api/signup — accepts JSON: { "email": "you@example.com" }
- GET  /api/emails — returns saved signups (local JSON file)

Deploy:
- Recommended: Render.com — connect your GitHub repo, create a Web Service, set Environment to Node, Branch to main, Build Command to `npm install`, and Start Command to `node server.js`.

Notes:
- This demo stores emails in a flat JSON file — not suitable for production. Use a database for real deployments.
- If you want me to add a password-protected admin page, convert the API to serverless for Vercel, or set up CI/CD, tell me and I will prepare the changes.
