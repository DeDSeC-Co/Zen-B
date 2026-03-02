Zen-B (Zen-Basket)

Zen-B is a full-stack e-commerce application built using Spring Boot + React, designed to simulate a real-world online shopping platform with customer and admin roles.

This project was built for learning and resume demonstration purposes, showcasing backend architecture, REST API design, authentication, and frontend integration.

🚀 Tech Stack
Backend

☕ Java 17

🌱 Spring Boot

🔐 JWT Authentication (Token via Cookies)

🗄 MySQL

📦 Maven

🐳 Docker

Frontend

⚛ React

⚡ Vite

🎨 HTML5 / CSS3

🟢 Node.js

🧩 Features

User & Admin Authentication

JWT-based authentication stored in HTTP-only cookies

Product browsing

Order placement & tracking

RESTful API architecture

MySQL persistent storage

Dockerized backend support

🏗 System Architecture
React (Vite)
     ↓
Spring Boot REST API
     ↓
MySQL Database
🔐 Authentication Flow

User logs in

Backend generates JWT

Token stored in secure HTTP-only cookie

Protected routes validated via filter

🖥 Running the Project
🔹 Backend
Option 1 — Run with Docker

Build image:

docker build -t zenb .

Run container:

docker run --name zenb-container -p 9090:9090 \
-e SERVER_PORT=9090 \
-e SPRING_DATASOURCE_URL=jdbc:mysql://host.docker.internal:3306/orbix \
-e SPRING_DATASOURCE_USERNAME="your_mysql_username" \
-e SPRING_DATASOURCE_PASSWORD="your_mysql_password" \
zenb

Backend runs on:

http://localhost:9090
Option 2 — Run via Spring Tools

Import project into Spring Tool Suite / IntelliJ

Wait for Maven dependencies to load

Run as Spring Boot Application

🔹 Frontend
npm install
npm run dev

Frontend runs on:

http://localhost:5173
🗄 Database Setup

Ensure MySQL is running

Create database:

CREATE DATABASE orbix;

Update credentials in environment variables

📂 Project Structure
Zen-B/
 ├── Zen-B_Backend/
 └── Zen-B_Frontend/
🎯 Purpose of the Project

Zen-B was developed to:

Demonstrate full-stack integration

Implement secure authentication using JWT

Showcase REST API design

Practice Docker containerization

Build production-style project structure
