# Wasm Minecraft Server

This project allows you to run a Wasm Minecraft client using a lightweight Nginx server within a Docker container.

## Pre-requisites

- Docker
- Docker Compose

## Getting Started

### Running with Docker Compose

We have configured a `docker-compose.yml` file for easy deployment. It sets up an Nginx server on port **3001** and limits container memory usage to **50MB**.

1.  **Build and Start the Container:**

    ```bash
    docker-compose up -d --build
    ```

2.  **Access the Application:**

    Open your browser and navigate to: [http://localhost:3001](http://localhost:3001)

3.  **Stop the Container:**

    ```bash
    docker-compose down
    ```

## Configuration Details

-   **Web Server:** Nginx (Alpine Linux based)
-   **Port:** 3001 (Mapped to internal port 80)
-   **Memory Limit:** 50MB
