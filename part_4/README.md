# Using Docker Compose to create a two tier application


### What did I do?

* I defined images using dockerfiles for:  
	* [mongodb](https://github.com/Benoniy/eng84_docker/blob/main/part_4/mongod/Dockerfile) - [benranson/mongod](https://hub.docker.com/repository/docker/benranson/mongod)
	* [nodejs app](https://github.com/Benoniy/eng84_docker/blob/main/part_4/webapp/Dockerfile) - [benranson/webapp](https://hub.docker.com/repository/docker/benranson/webapp)  


* I created a [docker-compose.yml](https://github.com/Benoniy/eng84_docker/blob/main/part_4/docker-compose.yml) that defines:
	* The creation of containers based on images
	* The creation of images if they dont exist
	* Environment variables


* I created a volume for persistent data that may not be visible here  
  although you can see the code for it in the [docker-compose.yml](https://github.com/Benoniy/eng84_docker/blob/main/part_4/docker-compose.yml)

