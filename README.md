# 1. Use Docker for Local Development

Containerized a Node.js application with Docker and ran it locally alongside a MongoDB database and a Mongo Express admin UI.

**Tech:** Docker · Node.js · MongoDB · Mongo Express

<br>

## What I did

- Created a Dockerfile for a Node.js application and built a Docker image
- Ran the Node.js app in a Docker container and connected it to a MongoDB database container locally
- Ran a Mongo Express container as a UI for the MongoDB database

<br>

## Architecture:

<img src="images/architecture.drawio.png" alt="">

## MongoDB + Mongo Express:

<img src="images/mongo-express.png" alt="">

<img src="images/mongo-express-2.png" alt="">

## Running App:

<img src="images/app.png" alt="">

<br>

# 2. Docker Compose - Run multiple Docker containers

This project uses Docker Compose to run MongoDB and Mongo Express together with a single configuration file.

**Tech:** Docker · MongoDB · Mongo Express

<br>

## What I did

- Wrote a Docker Compose file to configure and run the MongoDB and Mongo Express containers
- Defined the services, ports, and environment variables needed for the containers to communicate

<br>

<img src="images/start-container.png" alt="">

<br>

<img src="images/connection-established.png" alt="">

<br>

# 3. Dockerize Nodejs application

Dockerized a Node.js application by building and running it as a container.

**Tech:** Docker · Node.js

<br>

## What I did

- Wrote a Dockerfile to build a Docker image for the Node.js application
- Ran the application in a Docker container

<br>

<img src="images/build-docker-image.png" alt="">

<br>

<img src="images/docker-image.png" alt="">

<br>

<img src="images/app-listening.png" alt="">

<br>

# 4. Create Docker repository on Nexus and push to it

Created a private Docker registry on Nexus and pushed a Docker image to it from a DigitalOcean server.

**Tech:** Docker · Nexus · DigitalOcean · Linux

<br>

## What I did

- Created a hosted Docker repository and a Docker repository role in Nexus
- Created a Nexus user with permission to push images to the repository
- Connected Nexus, a DigitalOcean Droplet, and Docker so the server could authenticate with the registry
- Built and pushed a Docker image to the Nexus repository

<br>

<img src="images/push-image.png" alt="">

_Docker image being pushed to the Nexus repository._

<br>

<img src="images/image-in-nexus.png" alt="">

_Docker image successfully available in the Nexus repository._

<br>

# 5. Deploy Docker application on a server with Docker compose

Deployed a Docker Compose application to a remote server, including the Node.js app, MongoDB, and Mongo Express.

**Tech:** Docker · Node.js · MongoDB · Mongo Express

<br>

## What I did

- Copied the Docker Compose configuration to the remote server
- Logged in to the private Docker registry so the server could pull the application image
- Started the application, MongoDB, and Mongo Express services with Docker Compose
- Verified that the deployed application and database services were running successfully

<br>

<img src="images/app-deployed.png" alt="Docker Compose logs showing the deployed services running">

_Docker Compose services running on the remote server._

<br>

<img src="images/app-verification.png" alt="Mongo Express showing data from the deployed MongoDB database">

_Application data verified through Mongo Express after deployment._

<br>

<img src="images/framework.png" alt="Diagram of the Docker image build and deployment workflow">

_Overview of the build, registry, and deployment workflow._

<br>

# 6. Pesist data with Docker Volumes

Persisted MongoDB data outside the container by attaching a Docker volume to the database service.

**Tech:** Docker · Node.js · MongoDB

<br>

## What I did

- Created and attached a Docker volume to the MongoDB container
- Mounted the volume at MongoDB's data directory so database files are stored independently of the container
- Verified that the same data is available from both the Docker volume and the running MongoDB container

<br>

<img src="images/local-data.png" alt="MongoDB data files stored in the local Docker volume">

*MongoDB data files persisted in the local Docker volume.*

<br>

<img src="images/container-data.png" alt="MongoDB data files available inside the running container">

*The same persisted data is available inside the MongoDB container.*
