# Simple-3-Tier-Architecture-with-Docker-Compose

Welcome to Simple-3-Tier-Architecture-with-Docker-Compose repository! This project demonstrates how to set up a simple 3-tier architecture using Docker containers, including a frontend application, a backend API, and a MySQL database.

## Overview

The project is structured into three main components:

1. **Frontend**: A simple HTML web page served by an Apache HTTP Server container.
2. **Backend**: A PHP-based API running on an Apache server container, connected to a MySQL database.
3. **Database**: A MySQL database container initialized with a sample SQL dump.

Additionally, we include phpMyAdmin for easy database management.

## Prerequisites

Before you start, ensure you have the following:

- A reliable internet connection
- Docker installed on your machine. You can verify this by running the following commands:
  ```sh
    docker version
    docker compose version
## Getting Started
### Clone the Repository
    git clone https://github.com/ahmed1958/Simple-3-Tier-Architecture-with-Docker-Compose.git
    cd Simple-3-Tier-Architecture-with-Docker-Compose
### Project Structure
```bash
.
├── api                     
│   ├── app
│   │   ├── config.php      
│   │   ├── Database.php    
│   │   └── todos.php       
│   └── index.php           
├── db                      
│   └── dump.sql            
├── frontend                
│   └── index.html          
├── docker-compose.yml      
└── Dockerfile              
```


## Running the Containers
    docker compose up

  This command will start all the services defined in the docker-compose.yml file.
## Accessing the Services
  - **Frontend Application**: http://localhost:3000
  - **Backend API**: http://localhost:5000
  - **phpMyAdmin**: http://localhost:8080 (Username: todo_admin, Password: password)

## Acknowledgements 

  -**Special thanks to the open-source community for providing the tools and frameworks used in this project.**

  -****Note**: I did not write the code for the frontend and backend. My contribution was to Dockerize the project to demonstrate a 3-tier architecture using Docker containers.**
