# 🎬 Movie Review Web App

A full-stack web application built using **React**, **Spring Boot**, and **MongoDB** that allows users to browse movies, view trailers, and submit reviews. This project demonstrates best practices in building a RESTful API, integrating a NoSQL database, and creating a responsive frontend interface.

---

## 🛠️ Tech Stack

| Layer        | Technology                                                                 |
|--------------|----------------------------------------------------------------------------|
| **Frontend** | React.js, Axios, Bootstrap, Material UI, React Router, Font Awesome       |
| **Backend**  | Java, Spring Boot (REST API), Spring Data MongoDB                         |
| **Database** | MongoDB Atlas (Cloud-based NoSQL)                                         |
| **Tools**    | MongoDB Compass, Postman, VS Code, Git                     |

---

## ✅ Features

- 🎞️ Movie carousel with backdrop images and trailers
- 🧩 Modular frontend with React components
- 🔗 Spring Boot REST APIs with secure MongoDB connectivity
- 📝 Submit and view user reviews per movie
- 📦 .env file support for environment-based configurations
- 🔐 Secure database credentials via environment variables
- 🌐 Routing with `react-router-dom`

---

## 📂 Project Structure

📁 backend (Spring Boot API)
   └── MoviesController, ReviewsController
   └── MongoDB Models: Movie, Review
   └── MongoTemplate & Repository Setup

📁 frontend (React)
   └── Components: Hero, Header, Reviews, ReviewForm, Trailer
   └── Axios Configuration
   └── Material UI Carousel, React Router Integration

---

## 🔧 Step-by-Step Implementation

### 1. 📦 Backend Setup (Spring Boot + MongoDB)

- Initialized Spring Boot with Maven
- Added dependencies: `spring-boot-starter-data-mongodb`, `spring-boot-starter-web`, `lombok`
- Created MongoDB models: `Movie`, `Review`
- Built REST APIs for:
  - `GET /api/v1/movies` — fetch all movies
  - `GET /api/v1/movies/{imdbId}` — fetch movie by IMDb ID
  - `POST /api/v1/reviews` — add a review

### 2. ☁️ MongoDB Atlas Integration

- Created cloud MongoDB cluster on [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
- Imported movie data from JSON using MongoDB Compass
- Configured secure access and IP whitelisting
- Linked Spring Boot via URI in `.env`

### 3. 💻 Frontend Development (React)

- Bootstrapped React app using `create-react-app`
- Installed libraries:
  - `axios` for API requests
  - `react-router-dom` for routing
  - `react-bootstrap` and `bootstrap` for styling
  - `@mui/material`, `@emotion/react`, `react-player`, `font-awesome`
- Created components:
  - `Hero` — Carousel for featured movies
  - `Trailer` — Plays YouTube trailers
  - `Reviews` — Displays and submits reviews

### 4. 🌐 API Integration & Routing

- Configured Axios base URL
- Created reusable API functions
- Set up routing:
  - `/` — Home
  - `/Trailer/:ytTrailerId`
  - `/Reviews/:imdbId`

---

