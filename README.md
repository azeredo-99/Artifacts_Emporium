# Artifacts Emporium 🏛️

> Full-stack web application for discovering museums, exploring cultural events and purchasing museum tickets.

## 📌 About the Project

**Artifacts Emporium** is a full-stack web application developed as part of a university project.

The platform provides users with a way to explore museums and cultural events, view museum information and purchase tickets through an integrated web interface.

The project combines a frontend built with HTML, CSS and JavaScript with a Node.js/Express backend and a SQLite database.

The application is available in both **Portuguese and English**.

---

## ✨ Features

### 🏛️ Museum Exploration

Users can browse available museums and access detailed information about each location.

The platform includes dedicated pages for different museums and provides information about their collections and exhibitions.

### 🎫 Ticket System

Users can browse available tickets and purchase them through the platform.

The application also provides access to ticket and purchase information.

### 🔐 User Authentication

The application includes user registration and login functionality.

Authentication is handled by the backend using JSON Web Tokens (JWT).

### 🔎 Search

Users can search for museums and access relevant results through the search functionality.

### 📊 User Dashboard

The application provides user-related functionality, including access to purchase information and previously acquired tickets.

### 🌍 Multilingual Interface

The platform provides both:

- 🇵🇹 Portuguese
- 🇬🇧 English

versions of the main website pages.

---

## 🏗️ Architecture

The project follows a simple full-stack architecture:

```text
Frontend
   │
   │ HTTP Requests
   ▼
Node.js + Express
   │
   ├── REST API
   ├── Authentication
   └── Business Logic
          │
          ▼
       SQLite
```

The frontend communicates with the Express backend to retrieve and manipulate application data.

---

## 🛠️ Technologies

### Frontend

- HTML5
- CSS3
- JavaScript

### Backend

- Node.js
- Express.js
- CORS
- JSON Web Tokens (JWT)

### Database

- SQLite

### Development

- Git
- GitHub
- Visual Studio
  
---

## 🔌 Backend API

The Express backend provides API endpoints used by the frontend to communicate with the database.

The API handles functionality related to:

- Users
- Authentication
- Museums
- Search
- Tickets
- Purchases
- Visit tracking

The backend uses SQLite for persistent data storage.

---

## 🔐 Authentication

User authentication is implemented using **JSON Web Tokens (JWT)**.

The authentication flow allows users to:

1. Create an account
2. Log in
3. Receive an authentication token
4. Access authenticated functionality
5. Interact with user-specific data

---

## 🗄️ Database

The application uses **SQLite** as its database.

The database stores information required by the application, including:

- Users
- Museums
- Tickets
- Purchases
- Visits

The backend accesses the database through the `sqlite3` Node.js package.

---

## ▶️ Running the Project

### 1. Clone the repository

```bash
git clone https://github.com/azeredo-99/Museum-PWeb.git
cd Museum-PWeb
```

### 2. Install dependencies

```bash
npm install
```

### 3. Start the backend

```bash
node server.js
```

The Express server runs on:

```text
http://localhost:3000
```

### 4. Start the frontend

The frontend is composed of static HTML, CSS and JavaScript files.

It can be opened using a local development server such as **Live Server**.

For example:

```text
http://localhost:5500
```

The frontend communicates with the backend running on port `3000`.

---

## 🔄 Application Flow

A typical interaction with the platform follows this structure:

```text
User
 │
 ▼
Frontend
 │
 ├── Browse museums
 ├── Search
 ├── View museum information
 ├── Browse tickets
 └── Login / Register
 │
 ▼
Express API
 │
 ├── Authentication
 ├── Museum data
 ├── Ticket data
 └── Purchase data
 │
 ▼
SQLite Database
```

---

## 🎓 Academic Project

This project was developed as part of a university web programming project.

The main objective was to apply full-stack web development concepts, including:

- Frontend development
- Backend development
- REST APIs
- Database integration
- Authentication
- Client-server communication
- JavaScript programming

---

## 🚧 Future Improvements

Possible improvements for future versions include:

- [ ] Improve responsive design
- [ ] Improve frontend architecture
- [ ] Add automated tests
- [ ] Improve authentication security
- [ ] Move sensitive configuration to environment variables
- [ ] Improve API documentation
- [ ] Add stronger input validation
- [ ] Improve database management
- [ ] Deploy the application

---

## 👤 Author

### Guilherme Azeredo

Computer Systems Engineering graduate interested in software development, data and web technologies.

- GitHub: [azeredo-99](https://github.com/azeredo-99)
- LinkedIn: [Guilherme Azeredo](https://www.linkedin.com/in/gui-azeredo-a11bb0254/)

---

## 📄 License

This project was developed for educational and academic purposes.
