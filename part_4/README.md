# Using Docker Compose to create a two tier application


### What did I do?

* I defined images using dockerfiles for:  
	* mongodb  
	* nodejs app  


* I created a docker-compose.yml that defines:
	* The creation of containers based on images
	* The creation of images if they dont exist
	* Environment variables


* I created a volume for persistent data that may not be visible here  
  although you can see the code for it in the docker-compose.yml

