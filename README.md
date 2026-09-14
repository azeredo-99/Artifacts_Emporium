# Museum Ticketing Platform

A full-stack web app for discovering museums and buying tickets online, built with a course partner. Ten real museums (the British Museum, the Louvre, the Hermitage, the Prado, the Met, and others), each with its own page and payment flow, a shopping cart, and a bilingual Portuguese/English interface across every page.

## What it does

- **Browse & search** — a page per museum, plus a search page across all of them
- **Tickets & cart** — pick a ticket type, add it to a cart, pay, and see the order in a purchase history
- **Accounts** — register/login with JWT-based auth; purchase history is scoped to the logged-in user
- **Events** — a dedicated events listing alongside the permanent museum pages
- **PT/EN throughout** — every page exists twice, under `pages/PT` and `pages/ENG`
- **Basic site analytics** — a visit counter (`/increment-visit`, `/get-visits`, `/get-visits-this-month`)

## Architecture

```
index.html, login.js, register.js, results.js   # landing, auth and search entry points
pages/PT/, pages/ENG/    # one HTML page per museum + payment page, per language
js/                      # per-page client scripts (cart, checkout, search, per-museum logic)
css/                     # styles
database/database.db     # SQLite database
server.js                # Express API: auth, museums, tickets, purchase history, visit counts
```

## Tech stack

Node.js · Express · SQLite · JWT (`jsonwebtoken`) · HTML/CSS/JavaScript

## Running

```bash
npm install
node server.js
```
Then open `index.html` (or any page under `pages/PT` / `pages/ENG`) through a local server.

## Authors

Guilherme Azeredo & João Campos Cunha — [GitHub](https://github.com/azeredo-99) · [LinkedIn](https://www.linkedin.com/in/guilherme-azeredo-a11bb0254/)
