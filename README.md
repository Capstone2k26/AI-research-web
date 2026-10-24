# Smart Search v2

Smart Search v2 is a full-stack search application designed to rank results by trust, detect conflicting sources, and synthesize more reliable responses from available data.

## Overview

This project combines a Node.js/Express backend with a lightweight frontend interface. It is built to evaluate multiple sources, score relevance and credibility, and highlight inconsistencies or stale information.

## Key Features

- Search query processing with relevance scoring
- Trust and reliability analysis for search results
- Conflict detection across sources
- Verified answer synthesis for higher-confidence responses
- Local JSON-backed data storage
- Python bridge for advanced scoring and analysis

## Project Structure

- `smart-search-v2/` — main application folder
- `smart-search-v2/backend/` — Express API, scoring logic, database, Python bridge
- `smart-search-v2/frontend/public/` — frontend HTML, JavaScript, and CSS
- `smart-search-v2/backend/tests/` — automated tests for key logic and stale search behavior

## Stack

- Frontend: HTML, CSS, JavaScript
- Backend: Node.js, Express
- Data layer: lowdb JSON storage
- Additional analysis: Python bridge integration

## Local Setup

1. Open a terminal in the project directory.
2. Navigate to the backend folder:

   ```bash
   cd smart-search-v2/backend
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Start the server:

   ```bash
   npm start
   ```

5. Open the frontend UI from the `frontend/public` folder or serve it through the app as configured by the project.

## Running Tests

From the backend directory:

```bash
npm test
```

For stale-search checks:

```bash
npm run test:stale-search
```

## Notes

This repository is intended for local development and evaluation. The project is organized as a modular search engine prototype and is suitable for experimentation, extension, and testing of trust-aware search behavior.
