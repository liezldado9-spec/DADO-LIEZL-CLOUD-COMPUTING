# Mission Reflection

This laboratory helped me understand more about containers and how they are used in cloud computing. Before doing the activity, I knew that Docker could be used to run applications, but I did not fully understand how it works compared to a Virtual Machine. A Virtual Machine runs a complete operating system, while a Docker container shares the host operating system and can start with less overhead. During the activity, I experienced this by pulling the Nginx image and creating a container using Docker.

One important thing I learned was port mapping. The command `-p 8080:80` connects port 8080 on the host to port 80 inside the Nginx container. Because of this, I was able to use `curl http://localhost:8080` and receive the Nginx HTML page. Seeing the “Welcome to nginx!” message helped me understand that the web server was successfully running inside the container.

I also learned how the Docker container lifecycle works. I used `docker ps` to check the running container, `docker stop nginx-server` to stop it, and `docker rm nginx-server` to remove it. Finally, I used `docker ps -a` to verify that the container was removed. Doing these commands one by one made it easier for me to understand how containers are managed.

Containerization can help developers and IT operations teams work together because applications and their dependencies can be packaged into containers. This can make applications easier to run consistently in different environments.

This laboratory also added another practical skill to my GitHub cloud computing portfolio. Laboratory 04 allowed me to practice Docker, Nginx deployment, container lifecycle management, and technical documentation. Overall, the activity gave me a better understanding of how containers can be used in cloud-native environments.

