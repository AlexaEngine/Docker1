# Dockerized Full-Stack MERN Application

This project demonstrates the development and deployment of a full-stack MERN (MongoDB, Express.js, React.js, Node.js) application using Docker. The application is containerized using Docker, with Docker Compose orchestrating the deployment of the front end, back end, and MongoDB services.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [Project Structure](#project-structure)
- [License](#license)

## Introduction

This project involves setting up and Dockerizing a full-stack MERN application. The application demonstrates the use of Docker containers to manage the different components of a MERN stack application efficiently. The front end is developed using React.js, while the back end is built with Node.js and Express.js, and MongoDB serves as the database.

## Features

- Full-stack MERN application
- Dockerized front-end, back-end, and database services
- Docker Compose for orchestration
- Sample API routes for CRUD operations
- Simple front-end to display data from the API

## Technologies Used

- MongoDB
- Express.js
- React.js
- Node.js
- Docker
- Docker Compose

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Docker installed on your machine
- Node.js and npm installed on your machine

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/dockerized-mern-app.git
    cd dockerized-mern-app
    ```

2. Navigate to the project directory:

    ```bash
    cd RA21.2
    ```

3. Install the necessary dependencies for the client and server:

    ```bash
    cd client
    npm install
    cd ../server
    npm install
    ```

## Running the Application

To run the application, use Docker Compose:

1. Navigate to the root directory of the project:

    ```bash
    cd ../
    ```

2. Run the following command to build and start the Docker containers:

    ```bash
    docker-compose up --build
    ```

3. The application will be available at:

    - Frontend: `http://localhost:3000`
    - Backend: `http://localhost:9000`
    - API Endpoint: `http://localhost:9000/data`

## Project Structure

```plaintext
RA21.2/
├── client/
│   ├── public/
│   ├── src/
│   │   ├── App.css
│   │   ├── App.js
│   │   ├── index.css
│   │   ├── index.js
│   ├── Dockerfile
│   ├── package.json
├── server/
│   ├── routes/
│   ├── server.js
│   ├── Dockerfile
│   ├── package.json
├── docker-compose.yml

License
This project is licensed under the MIT License. See the LICENSE file for details.
### Explanation:
- **Introduction:** Provides a brief overview of the project.
- **Features:** Lists the key features of the project.
- **Technologies Used:** Lists the main technologies used in the project.
- **Prerequisites:** Specifies the requirements to run the project.
- **Installation:** Provides step-by-step instructions to install the project dependencies.
- **Running the Application:** Details how to build and run the Docker containers for the application.
- **Project Structure:** Shows the directory structure of the project.
- **License:** States the licensing information for the project.

