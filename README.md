# Rust + PostgreSQL Docker Configuration
An easy to setup Docker configuration for Rust and PostgreSQL database.

### Built With
* [![Docker][Docker-shield]][Docker-url]
* [![Rust][Rust-shield]][Rust-url]

## Getting Started
This is the guide for setting up a local dev environment. The Rust Docker container starts with the `cargo watch` parameter, so it builds automatically after project changes and displays build errors, warnings, etc. in the container logs.

### Prerequisites
Before the installation, you should have a Docker Engine installed. 

_For Docker installation guide, please refer to the [Official Docker Guide](https://docs.docker.com/get-started/get-docker/)_.

### Installation
1. Clone the repo
    ```shell
    git clone https://github.com/reclikp/rust-postgres-docker.git
    ```
2. Navigate to your directory
    ```shell
    cd your_directory/rust-postgres-docker
    ```
3. Remove current git configuration 
    ```shell
   rm -rf ./.git
    ```
4. Create project .env file
    ```shell
    cp ./.env.example .env
    ```
5. Set your configuration
    ```dotenv
    # .env
    POSTGRES_USER=your_database_user
    POSTGRES_PASSWORD=your_database_password
    POSTGRES_DB=your_database_name
    ```
6. Build and start the project
    ```shell
   docker compose up
    ```
7. Enjoy your Rust project. By default the project starts with _cargo watch_ so you can debug your logs. ;)

[Docker-shield]: https://img.shields.io/badge/docker-000000?style=for-the-badge&logo=docker&logoColor=blue
[Docker-url]: https://www.docker.com/
[Rust-shield]: https://img.shields.io/badge/rust-000000?style=for-the-badge&logo=rust&logoColor=red
[Rust-url]: [https://www.docker.com/](https://www.rust-lang.org/)
