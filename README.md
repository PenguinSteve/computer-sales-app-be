# Computer Sales Backend

## Project Overview

This project is a backend system for a computer sales application. It provides APIs and services to manage orders, inventory, and user interactions. The system is designed to be scalable and efficient, leveraging modern technologies and best practices.

## Features

-   **Order Management**: Handles order creation, updates, and notifications.
-   **Inventory Management**: Tracks stock levels and updates in real-time.
-   **Email Notifications**: Sends order confirmation and status updates to customers.
-   **Queue System**: Uses Redis for managing background tasks and job queues.
-   **Database Integration**: MongoDB for storing and managing data.

## Technologies Used

-   **Node.js**: Backend runtime environment.
-   **TypeScript**: Strongly typed programming language for better code quality.
-   **Express.js**: Web framework for building APIs.
-   **MongoDB**: NoSQL database for data storage.
-   **Redis**: In-memory data structure store for caching and job queues.
-   **Docker**: Containerization for consistent development and deployment environments.
-   **Docker Compose**: Orchestrates multi-container Docker applications.
-   **Elasticsearch**: Used for enhancing search performance and scalability.

## Setup Instructions

### Prerequisites

-   Install [Docker](https://www.docker.com/) and [Docker Compose](https://docs.docker.com/compose/).
-   Install [Node.js](https://nodejs.org/) and npm.

### Steps to Run the Project

1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd computer-sales-be
    ```
2. Create a `.env` file in the root directory and configure the following variables:
    ```env
    REDIS_URL=redis://localhost:6379
    MONGO_URL=mongodb://localhost:27017/computer-sales
    ELASTICSEARCH_HOST=http://elasticsearch:9200
    ```
3. Build and start the project using Docker Compose:
    ```bash
    docker compose up -d --build
    ```
### Cleaning and Rebuilding

To clean and rebuild the project:

```bash
npm cache clean --force
rm -rf node_modules
npm install
npm run build
```

## Additional Notes

-   Ensure that the `REDIS_URL` and `MONGO_URL` in the `.env` file are correctly configured.
-   Use `docker logs <container_name>` to debug any issues with Docker containers.

## License

This project is licensed under the MIT License.
