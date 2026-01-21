# AWESOME PIZZA - INFRASTRUCTURE
In this repository we can find every necessary configuration needed to create the following architecture:

![architecture](https://github.com/Rabberpoli/awesome-pizza-infrastructure/blob/main/awesome-pizza-architecture.svg)

## Technology stack:
The following technologies were used:
* **ReactJS 19** (with TS extension) + **Vite** (for bundling)
* **Java 17** + **Springboot 3** + **Maven** (for dependencies management and build)
* **Redis** (queue structure)
* **SockJS** (websocket infrastructure for real-time notifications)
* **Docker** (containerization)

## Project setup
In order to use this simple web-app you two options:
1. Build each image using the `Dockerfile` you will find in [client](https://github.com/Rabberpoli/awesome-pizza-client) and [service](https://github.com/Rabberpoli/awesome-pizza-service) repos
2. Starting directly with `docker-compose.yaml` (images are already pushed to my personal dockerHub, so you don't have to build it on your own)
