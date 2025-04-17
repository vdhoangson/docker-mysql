# Docker MySQL Setup

This project sets up a MySQL 8.0 database using Docker Compose.

## Features

- MySQL 8.0
- Environment variables for user and password configuration
- Persistent data storage using Docker volumes

## Prerequisites

- Docker
- Docker Compose

## Setup

1. Clone this repository.
2. Create a `.env` file based on the provided `.env.example` file:
   ```bash
   cp .env.example .env
   ```
3. Update the `.env` file with your desired MySQL user and password.

## Usage

Start the MySQL container:

```bash
docker-compose up -d
```

Access the MySQL database on `localhost:3306` using the credentials specified in the `.env` file.

## Volumes

The database data is stored persistently in the `db_data` volume.

## Stopping the Container

To stop the container, run:

```bash
docker-compose down
```

## License

This project is licensed under the MIT License.
