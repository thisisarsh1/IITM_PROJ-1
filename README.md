# iitm\_proj\_1 - FastAPI Application with Uvicorn

This repository provides a Dockerized FastAPI application that runs using Uvicorn.

## Prerequisites

Before starting, ensure you have the following installed:

- [Docker](https://docs.docker.com/get-docker/)

## Running Locally with Docker

To build and run the application locally:

### 1. Clone the repository (if not already done)

```sh
git clone <repository-url>
cd <repository-folder>
```

### 2. Build the Docker Image

```sh
docker build -t iitm_proj_1 .
```

### 3. Run the Container

```sh
docker run -p 8000:8000 iitm_proj_1
```

### 4. Access the Application

Once the container is running, access the FastAPI application at:

- [http://localhost:8000](http://localhost:8000)
- Swagger UI: [http://localhost:8000/docs](http://localhost:8000/docs)

## Running from Docker Hub

If you want to pull and run the image from Docker Hub:

### 1. Pull the Image

```sh
docker pull theklausmikaelson/iitm_proj_1:v2
```

### 2. Run the Container

```sh
docker run -p 8000:8000 theklausmikaelson/iitm_proj_1:v2
```

## Stopping the Container

To stop the running container, find its `CONTAINER ID` using:

```sh
docker ps
```

Then stop it using:

```sh
docker stop <CONTAINER_ID>
```

## License

This project is open-source under the MIT License.

