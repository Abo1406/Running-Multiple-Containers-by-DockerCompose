# Running-Multiple-Containers-by-DockerCompose
# MongoDB with Mongo Express - Docker Compose Setup

This repository contains a `mongo.yaml` file to set up a **MongoDB** database along with **Mongo Express**, a web-based MongoDB administration interface.

## Prerequisites

Ensure you have the following installed on your system:
- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Getting Started

### Clone the Repository
```sh
git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPOSITORY_NAME.git
cd YOUR_REPOSITORY_NAME
```

### Run the Containers
Use the following command to start the MongoDB and Mongo Express services:
```sh
docker-compose up -d
```
This will run the services in detached mode (`-d`).

### Services and Ports
- **MongoDB** is available on port `27017`.
- **Mongo Express** is accessible via `http://localhost:5000`.

### Environment Variables
The services are configured with the following environment variables:

#### **MongoDB**
| Variable | Value |
|----------|-------|
| MONGO_INITDB_ROOT_USERNAME | `abmrv` |
| MONGO_INITDB_ROOT_PASSWORD | `123` |

#### **Mongo Express**
| Variable | Value |
|----------------------------------|------------|
| ME_CONFIG_MONGODB_ADMINUSERNAME | `admin` |
| ME_CONFIG_MONGODB_ADMINPASSWORD | `password` |
| ME_CONFIG_MONGODB_SERVER | `mongodb` |

### Stopping the Containers
To stop the running containers, use:
```sh
docker-compose down
```
This will stop and remove the containers.

## Contributing
Feel free to fork this repository and submit a pull request with improvements or new features!

## License
This project is licensed under the MIT License.

