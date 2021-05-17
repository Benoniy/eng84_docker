### What is Docker?  
    Docker is a containerisation tool that enables developers to seperate their applications from their  
    infrastructure. It does this by utilising containers.  
    Containers images are lightweight, standalone, executable packages of software that include  
    everything needed to run an application: code, runtime, system tools, system libraries and settings.  


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
	* Industry standard
	* Efficient operation
	* Compatible with most industry tools
	* Easy 


### How is it different to a VM?  
	Containerisation is very simmilar to Virtualisation on the surface, however underneath the hood  
	there are some key differences.  


	* Run's on the host os' kernel rather than virtualising another one.  
	* Uses the User space of the existing operating system.  
	* Shares hardware resources instead of reserving them.  
	* It runs on the host so images are smaller and performance is more efficient.  


### Installation and Setup  
	Installation is easy, you just go to this [link](https://www.docker.com/products/docker-desktop) and click the download button!  


### DockerHub account and Repository  
	Docker has version control component that is very simmilar to GitHub, its called Docker Hub and it  
	allows us to create repositories to store our images in. You can create a repository directly from  
	the dockerhub webpage or automatically create one by pushing an image to a valid namspace.  


	* All docker repositories use the format `username/repo_name`, this is the name you should push  
	  your images to.  
	

### Containers and Images  
	Containers - Isolated environments that run an instance of an image.  
	Images - A read only template that contains set instructions for creating a container.  


### Building images and microservices  
	Building an image is relativly simple.  


	After pulling an image and creating a container out of that image, you can simply do the following:   
		1. `docker ps -a` - find the container id of the container you want to turn into an image  
		2. `docker commit <container_id> <name_of_repo>` - then commit it to a new image, note  
		   `<name_of_repo>` should contain `username/name`  
		3. `docker push <name_of_repo>:<tag>` - This pushes it, `<tag>` is usualy `latest`  


	***What are microservics?***  
	Microservices are tiny apps that are meant to do one thing only with as little context as possible.  
	Ideally they should perform only one task and stopping them should not affect any other workstream  
	or action.  


### What is Kubernetes (k8)? 
	Kubernetes is a containerisation orchestration tool that that facilitates both declarative  
	configuration and automation. It is widely available and enables convenient managment of a lot of  
	different containerisation services.  


### What are the benefits of K8?  
	* Widely available  
	* Self-healing
	* Secret and configuration managment
	* Automated rollout
	* Storage managment
	* Load balancing
