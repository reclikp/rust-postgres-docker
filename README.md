# Rust + PostgreSQL Docker Configuration

## Getting Started
Currently, configuration is working ONLY in a dev environment. Production deploy features should be added soon. ;)

### Installation

1. Clone the repo
    ```shell
    git clone https://github.com/reclikp/rust-postgres-docker.git
    ```
2. Navigate to your directory
    ```shell
    cd your_directory/rust-postgres-docker
    ```
3. Copy .env.example
    ```shell
    cp ./.env.example .env
    ```
4. Set your configuration
    ```dotenv
    # .env
    POSTGRES_USER=your_database_user
    POSTGRES_PASSWORD=your_database_password
    POSTGRES_DB=your_database_name
    ```
5. Build and start the project
    ```shell
   docker compose up
    ```
6. Enjoy cargo watch logs and fix your errors ;)
