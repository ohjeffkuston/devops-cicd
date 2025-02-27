# DevOps Project: Deploy Docker Image to AWS EC2 using GitHub Actions

This project demonstrates a CI/CD pipeline that containerizes a simple Node.js web application, builds and pushes a Docker image to DockerHub, and deploys it to an AWS EC2 instance using GitHub Actions.

## Overview

- **Application**: A lightweight Node.js web app using Express, running on port 3000.
- **Containerization**: Dockerized with a custom `Dockerfile`.
- **Infrastructure**: AWS EC2 instance running Amazon Linux 2 with Docker installed.
- **CI/CD**: GitHub Actions workflow to build, push, and deploy the Docker image on every push to the `main` branch.
- **Access**: Deployed app accessible via the EC2 public IP on port 3000.

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/) installed locally.
- [AWS CLI](https://aws.amazon.com/cli/) configured with credentials.
- A [DockerHub](https://hub.docker.com/) account.
- A GitHub repository for this project.
- An SSH key pair for EC2 access (e.g., `MyKeyPair.pem`)