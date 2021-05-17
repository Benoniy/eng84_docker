### What is Docker?  
	Docker is a containerisation tool


### Cheat Sheet:  
	* `docker --version` - Check the docker version


	* `docker pull img_name` - Pull an image off of DockerHub


	* `docker run img_name` - This will pull and then containerise an image
		* `-d` - Detached
		* `-p local_port:container_port` - Map a port 
		* `--name` - Name the container


	* `docker rmi -f img_name` - Delete an image `-f` is force


	* `docker ps -a` - List containers, `-a` is for all


	* `docker images` - List all images that are stored localy


	* `docker rm -f container_id` - Delete a container, `-f` is force


	* `docker start container_id` - Start up a container


	* `docker stop container_id` - Stop a running container


	* `docker exec -it container_id sh` - Connect to a container cli


	* `docker commit container_name username/new_img_id` - create a new image from a container


	* `docker push image_id`


### Why use Docker?  
	* Efficient
	* Compatible with most industry tools
	* Easy


### How is it different to a VM?  
	


### Installation and Setup  
	


### DockerHub account and Repository  
	


### Containers and Images  
	


### Building images and microservices  
	
