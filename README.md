# Dynamic Edge — Wholesale Website (Node.js)

A ready-to-run Node.js/Express wrapper for the responsive bilingual Arabic/English Dynamic Edge wholesale website. The original logo is embedded in the HTML, so no separate logo file is required.

## Requirements
- Node.js 20 or newer
- npm

## Run locally
1. Extract the project ZIP.
2. Open the extracted `dynamic-edge-node-project` folder in VS Code.
3. Open Terminal in VS Code and run:

   ```bash
   npm install
   npm start
   ```

4. Visit `http://localhost:3000`.
5. Health check: `http://localhost:3000/health`.

For development with Node's watch mode, run `npm run dev`.

## Deploy to Render
1. Create a Git repository and upload the contents of this folder to GitHub.
2. In Render, choose **New + → Web Service** and connect the repository.
3. Use these settings:
   - Runtime: Node
   - Build command: `npm install`
   - Start command: `npm start`
4. Deploy. Render supplies the `PORT` environment variable automatically.

A `render.yaml` Blueprint file is included as an alternative deployment configuration. Hosting providers and their free plans can change over time.

## Deploy to another Node host
Upload the project folder/repository, install dependencies with `npm install`, and start it with `npm start`. The app listens on `process.env.PORT` and binds to `0.0.0.0`.

## Important notes before publishing
- The contact form currently opens the visitor's default email app using `mailto:`. It does **not** save enquiries to a database or send email directly from the server. For dependable enquiries, connect a form/email provider or implement a secure backend email service.
- Confirm the displayed business email, address, branch details, manager name, product categories, shipping terms, and wholesale minimum order quantities before publishing.
- The project is a wholesale business website, not a full ecommerce checkout or inventory-management system.
