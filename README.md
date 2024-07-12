# Open Music API V3 - Consumer

Proyek ini adalah consumer untuk proyek [Open Music API V3](https://github.com/The-Aldi-Tri/open-music-api-v3).

## How to run

**Make sure project [Open Music API V3](https://github.com/The-Aldi-Tri/open-music-api-v3) are running in another Terminal/VS Code window.**

Create an **.env** file in the root directory of project and fill it with variables based on the examples in the **.env.example** file

### - Locally

- Prerequisites

  - **Node.js** installed on your local machine. You can download it from [nodejs.org](https://nodejs.org/).
  - **Postgresql** database installed on your local machine. You can download it from [postgresql.org](https://www.postgresql.org/download/).
  - **Redis** for caching installed on your local machine. You can download it from [redis.io](https://redis.io/downloads/).
  - **RabbitMQ** for message broker installed on your local machine. You can download it from [rabbitmq.com](https://www.rabbitmq.com/docs/download).

- Installation

  Clone the repository and install dependencies.

  ```bash
  git clone <repository-url>
  cd <project-directory>
  npm install
  ```

- Running

  Make sure you have started your database server and then run this

  ```bash
  npm start
  ```

### - DevContainer (Docker)

- Prerequisites

  Make sure you have the following installed:

  - **Visual Studio Code** ([VS Code](https://code.visualstudio.com/download))
  - **Docker** (Docker Engine with Compose plugin or [Docker Desktop](https://www.docker.com/products/docker-desktop/))
  - **Remote Development** extension pack for VS Code (Install from the VS Code Extensions marketplace)
  - **Docker Images** you can search in [Docker Hub](https://hub.docker.com/search)
    - Nodejs
    - Postgres
    - Redis
    - RabbitMQ

  Make sure you have Docker network named **my-network**. You can create this after installing docker with this command:
  ```bash
  docker network create -d bridge my-network
  ```

- Installation

  1. Clone the repository:

     ```bash
     git clone <repository-url>
     cd <project-directory>
     ```

  2. Open the project in VS Code

     Make sure docker is running.

  3. Reopen in Container:

     Once you have the Remote - Containers extension installed, you'll see a green Remote indicator in the bottom-left corner of the VS Code window.
     Click on the green indicator, or use Ctrl/Cmd + Shift + P to open the Command Palette and search for Remote-Containers: Reopen in Container.
     Select your desired development container configuration (e.g., Node.js), and VS Code will reopen the project inside the container.

  4. Open Terminal and run this

     ```bash
     npm install
     ```

- Running

  ```bash
  npm start
  ```
