# Project README

## Description

This project demonstrates the usage of Docker Compose to deploy a web application using Nginx and PHP containers. The Docker Compose file (`docker-compose.yml`) defines the services, their configurations, and the overall application setup. 

## Files

1. `docker-compose.yml`: 
   - Purpose: Defines the services, their configurations, and resource limits for the application.
   - Usage: Run `docker-compose up` to deploy the application stack.

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

5. Deploy the application:
- Run the following command to start the application stack:
  ```
  docker-compose up -d
  ```

6. Access the application:
- Open a web browser and navigate to `http://localhost` to access the deployed web application.

7. Cleanup:
- To stop and remove the application containers, run:
  ```
  docker-compose down
  ```

## Notes

- Ensure that Docker and Docker Compose are installed on your system before running the application.
- Make sure to customize the `index.php` and `app.conf` files according to your specific application requirements.
