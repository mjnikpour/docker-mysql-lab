# Run MySQL Container

## Pull the image
docker pull mysql

## Run the container
docker run -d --name my-mysql -e MYSQL_ROOT_PASSWORD=root123 -p 3306:3306 mysql

## Check running containers
docker ps

## Stop the container
docker stop my-mysql

## Remove the container
docker rm my-mysql

## Remove the image
docker rmi mysql

## Explanation
- -d runs the container in detached mode
- --name my-mysql sets a name for the container
- -e MYSQL_ROOT_PASSWORD=root123 sets the root password
- -p 3306:3306 maps MySQL port from container to host
