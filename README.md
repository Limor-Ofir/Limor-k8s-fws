# HOW TO RUN WORDPRESS APP WITH A DATABASE USING KUBERNETES
WordPress on Kubernetes
This repository contains the configuration files and instructions for deploying a WordPress application with a MariaDB database using Kubernetes. The setup includes using a StatefulSet for the database and an Ingress Controller for external access to the WordPress application.

## Prerequisites
1. A running Kubernetes cluster
2. kubectl command-line tool configured to access your cluster
3. Access to a cloud provider (if using LoadBalancer services)
4. Docker installed (for building images, if necessary)
5. Architecture Overview
6. MariaDB StatefulSet: Manages the database with persistent storage.
7. WordPress Deployment: Runs the WordPress application.
8. Ingress Controller: Provides external access to the WordPress application.
9. Persistent Volume Claims: Ensure data persistence for MariaDB.
10. Look at the Example Repository
 - The docker-compose you will be migrating from is in the following repository:
https://github.com/docker/awesome-compose/blob/master/official-
documentation-samples/wordpress/README.md
## Deployment Steps
### 1. Set Up MariaDB
#### Create a YAML file for the MariaDB StatefulSet

### 2. Create a Service for MariaDB
#### If there is no existing service, create one

### 3. Deploy WordPress
#### Create a YAML file for the WordPress deployment

### 4. Create a Service for WordPress
#### Create a service for the WordPress deployment

### 5. Set Up Ingress
#### Create an Ingress resource to expose WordPress

### 6. Apply the Configurations
#### Use kubectl to apply the YAML files

### 7. Verify the Deployment
#### Check the status of all resources

### 8. Access WordPress
#### You can access your WordPress installation through the domain or IP configured in your Ingress resource. Use nip.io for local testing with your LoadBalancer IP.

## Conclusion
This setup provides a robust WordPress installation on Kubernetes with a persistent database backend. You can modify the configurations as needed to suit your environment.

# GOOD LUCK :)
