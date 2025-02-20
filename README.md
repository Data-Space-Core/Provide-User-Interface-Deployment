# Provide User Interface Deployment

This documentation provides instructions on setting up and running the user interface for Data Provision in DSIL (Data Space Innovation Lab).


## Prerequisites
Before proceeding, ensure you have the following installed on your system:

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)
- [Running DISIL Connector](https://github.com/Data-Space-Core/Connector-Deployment)


## Configuration
The Provide User Interface is configured using an environment file (.env): 
- **Connector URL**: Set the `CONNECTOR_URL` to the desired URL of the connector service.
  ```env
  CONNECTOR_URL=http://localhost:8081


## Running the Service
1. Start the service:
   ```sh
   docker-compose up -d
   ```

## Checking if Running
1. Check running containers:
   ```sh
   docker ps
   ```
2. Access the application at:
   ```
   http://localhost:8000/provide/offer/
   ```

## Shutting Down
1. Stop the service:
   ```sh
   docker-compose down
   ```

