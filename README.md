# Simple Load Balancer and Reverse Proxy with Docker and Nginx

This project demonstrates how to set up a simple load balancer and reverse proxy using Docker and Nginx. The load balancer will distribute incoming requests to multiple backend services running in Docker containers.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Clone the Repository](#clone-the-repository)
  - [Build and Run the Containers](#build-and-run-the-containers)
  - [Access the Load Balancer](#access-the-load-balancer)

## Prerequisites

- Docker installed on your machine
- Docker Compose installed on your machine

## Project Structure

.  
├── docker-compose.yaml   
├── nginx.conf  
└── README.md  

- `docker-compose.yaml`: Docker Compose configuration file to set up the services.
- `nginx.conf`: Nginx configuration file for load balancing and reverse proxying.
- `README.md`: Project documentation.

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/luismunhoz55/simple_load_balancer.git
cd simple-load-balancer
```

## Build and Run the Containers
Run the following command to build and start the containers:

```bash
docker-compose up -d
```

This will start the Nginx load balancer and the backend services.

# Access the Load Balancer
You can access the load balancer and the services using the following URLs:

- For the blue service: http://blue.192.168.64.1.nip.io:8080
- For the green service: http://green.192.168.64.1.nip.io:8080
- For the conversion service: http://conversao.192.168.64.1.nip.io:8080
Make sure to replace 192.168.64.1 with your actual IP address if different.
