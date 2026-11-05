# 1. Use Docker for Local Development

Containerized a Node.js application with Docker and ran it locally alongside a MongoDB database and a Mongo Express admin UI.

**Tech:** Docker · Node.js · MongoDB · Mongo Express

<br>

## What I did

- Created a Dockerfile for a Node.js application and built a Docker image
- Ran the Node.js app in a Docker container and connected it to a MongoDB database container locally
- Ran a Mongo Express container as a UI for the MongoDB database

<br>

## Skills demonstrated

Containerization with Docker, Dockerfile authoring, multi-container local development, Docker networking, working with MongoDBd

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

<br>

<img src="images/image-in-nexus.png" alt="">
