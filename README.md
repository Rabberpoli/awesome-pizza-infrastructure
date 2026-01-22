# AWESOME PIZZA - INFRASTRUCTURE
In this repository we can find every necessary configuration needed to create the following architecture:

![architecture](https://github.com/Rabberpoli/awesome-pizza-infrastructure/blob/main/awesome-pizza-architecture.svg)

## Technology stack:
The following technologies were used:
* **ReactJS 19** (with TS extension) + **Vite** (for bundling)
* **Nginx** as a reverse proxy
* **Java 17** + **Springboot 3** + **Maven** (for dependencies management and build) + **H2** (embedded DB)
* **Redis** (queue structure)
* **SockJS** (websocket infrastructure for real-time notifications)
* **Docker** (containerization)

## Project setup
In order to run this simple web-app you 4 options:
1. Build each image using the `Dockerfile` you will find in [client](https://github.com/Rabberpoli/awesome-pizza-client) and [service](https://github.com/Rabberpoli/awesome-pizza-service) repos
2. Starting directly with `docker-compose.yaml` (images are already pushed to my personal dockerHub, so you don't have to build it on your own)
3. Access remotely on this [Google Cloud VM](http://35.222.70.118/) (this is a trial VM with no domain; IP is dynamic so it can change and I need to update it here)
4. Run components locally --> look at [client](https://github.com/Rabberpoli/awesome-pizza-client) and [service](https://github.com/Rabberpoli/awesome-pizza-service) README

## Useful resources
| Go to...                                    | and you'll find...                         |
| ------------------------------              | -----------------------------------------  |
| http://35.222.70.118/                       | **Awesome Pizza APP**                      |
| http://35.222.70.118/h2-console             | **H2 file based embedded DB**              |
| http://35.222.70.118/swagger-ui/index.html  | **Swagger interface with API description** |

> H2 console will ask you to insert some auth data. You just have to put this connection string `jdbc:h2:file:./data/awesome_pizza_db` and connect. You'll see all data and tables available.
