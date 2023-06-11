# Project README

## Description

This project demonstrates the usage of Docker Compose to deploy a web application using Nginx and PHP containers. The Docker Compose file (`docker-compose.yml`) defines the services, their configurations, and the overall application setup. 

## Files

1. `docker-compose.yml`: 
   - Purpose: Defines the services, their configurations, and resource limits for the application

2. `www/index.php`:
   - Purpose: Contains the PHP code for the web application.
   - Usage: Modify this file according to your application's requirements.

3. `nginx/app.conf`:
   - Purpose: Nginx configuration file that specifies how requests should be handled.
   - Usage: Customize this file to configure Nginx based on your application's needs.

## Usage

1. Clone the project repository:
git clone https://github.com/your/repository.git

2. Navigate to the project folder:

3. Modify `www/index.php`:
- Edit this file to add your PHP application logic and code.

4. Customize `nginx/app.conf`:
- Adjust the Nginx configuration in this file based on your application's requirements.

5. Deploy the services: 
- Run the following command to deploy the services defined in the Docker Compose file:
  ```
  docker stack deploy -c docker-compose.yml <STACKNAME>
  ```
6. Verify the deployment: Use the following commands to check the status and logs of the deployed services:
- To check the status of the stack:
  ```
  docker stack ps <STACKNAME>
  ```
- To view the logs of the NGINX service:
  ```
  docker service logs <STACKNAME>_nginx
  ```
- To view the logs of the PHP service:
  ```
  docker service logs <STACKNAME>_php
  ```
7. Access the application:
- Open a web browser and navigate to `http://localhost` to access the deployed web application.

8. Cleanup:
- To stop and remove the application containers, run:
  ```
  docker stack rm <STACKNAME>
  ```
