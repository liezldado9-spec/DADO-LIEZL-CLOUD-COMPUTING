# Mission Reflection

This lab helped me gain insight into containers and their utilisation in the cloud computing world. Prior to doing the activity I knew that I could use Docker to run an application, but I didn't completely understand how Docker works versus a Virtual Machine. A Virtual Machine is a full OS with full OS boot overhead, whereas a Docker container is a container of the host OS with reduced boot overhead. I had to do this during the activity, when I pulled the image of Nginx and created a container with Docker.

One of the lessons I learned is port mapping. The -p 8080:80 exposes the port 80 in Nginx to port 8080 on the host. As a result, I was able to curl http://localhost:8080 and get the Nginx HTML screen. Seeing the “Welcome to nginx!” message helped me understand that the web server was successfully running inside the container.

I also gained an understanding of the lifecycle of a Docker container. To check the running container I used docker ps, to stop it, I used docker stop nginx-server, and to remove it, I used docker rm nginx-server. Lastly, I confirmed the container was deleted with docker ps -a. Doing these commands one by one made it easier for me to understand how containers are managed.

Applications and their dependencies can be packaged into containers, enabling developers and IT operations teams to work together on containers. This can make applications more consistent to run across environments.

Another practical skill was added to my GitHub cloud computing portfolio in this lab. I got a chance to practice Docker, Nginx deployment, container lifecycle management and technical documentation in lab 04. Overall, it helped me to understand the use of containers in cloud-native environments better.
