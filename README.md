Setup a Docker environment for a Laravel Jetstream application using a LEMP
stack. The Dockerfile sets up the PHP environment, while the compose.yml file
defines the services and their configurations. We also configured Nginx to serve
the Laravel application.

Best practices include using environment variables for sensitive data, mapping
volumes for code and database persistence, and ensuring all necessary PHP
extensions are installed. This setup allows for easy management and deployment
of the Laravel application in a containerized environment.

# Start the app

### sudo docker compose up --build --wait -d

### docker exec -it jetstream_app php artisan migrate

#### For permission issues: chown all files to www-data:www-data inside the docker container