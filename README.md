# Provide User Interface Deployment Using Docker

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
  CONNECTOR_URL=https://localhost:8081/
  ```

## Running the DSIL Connector Provider Interface
Follow these steps to start the services using Docker Compose:

https://github.com/Data-Space-Core/Provide-User-Interface-Deployment.git
1. **Clone the repository**
   ```
   git clone https://github.com/Data-Space-Core/Provide-User-Interface-Deployment.git
   ```
2. **Navigate to the project directory**
   ```
   cd /Provide-User-Interface-Deployment
   ```
3. **Start the containers**
   ```
   docker compose up --build -d
   ```
4. **Verify running containers**
   ```
   docker ps
   ```
5. **Check logs if needed**
   ```
   docker compose logs -f <container-id>
   ```
   
6. **Access DSIL Connector Provider Interface application**
   ```
   http://localhost:8000/
   ```

## Stopping the Services
To stop and remove the running containers, run:
```sh
docker compose down -v
```

