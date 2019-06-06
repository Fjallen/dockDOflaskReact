# Microservices with Docker, Flask, and React

[![Build Status](https://travis-ci.org/fjallen/dockDOflaskReact.svg?branch=master)](https://travis-ci.org/fjallen/dockDOflaskReact)

### Testing out Docker React and Flask with Kubernetes deployed on Digital Ocean

# Production Server Live At presentr.ca
When everything works in Development but breaks in production... Production server is currently not working properly and error 500 is ...

# Important Lessons from Doing This

* Creating a bunch of tiny changes and building it with Docker-Compose eats up storage space.
* Check Docker Images with Docker Images once in a while and clear up the storage using docker rmi image-name
* When using VirtualBox, make sure to allocate at loeast 10 GB, recommened 20 Gb to a Ubuntu image. Doing development in this instance eats up so much storage, and when Ubuntu runs out of storage, well..., good thing you're working with a Virtual Machine, so you can just remove it
* Make sure you docker-compose up -d before using npm start, since server won't just be on in the background
