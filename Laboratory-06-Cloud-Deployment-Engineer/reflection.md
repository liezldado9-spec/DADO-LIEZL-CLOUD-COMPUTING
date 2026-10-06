# Mission 6 Reflection

For me, writing the docker-compose.yml file made the deployment easier because I only needed one file to set up the different containers. Instead of typing many commands one by one, I could put the settings for Nextcloud and MariaDB in the file and run them together. This made the process faster and more organized.

I learned that YAML needs the correct indentation. If I use a Tab or put the spaces in the wrong place, Docker Compose may show an error and the containers may not start. While doing this activity, I understood why the format of the file is important.

We used environment variables like MYSQL_PASSWORD because they provide the information needed for Nextcloud to connect to the MariaDB database. The database name, username, password, and host were included so the two containers could communicate properly.

I felt happy when I saw that both the Nextcloud and MariaDB containers were running successfully. At first, I was a little worried about making mistakes in the YAML file, but seeing the Nextcloud setup page made me feel that I was able to complete the deployment correctly.

Since Mission 1, my understanding of Cloud Computing has improved. Before, I mainly understood cloud computing as using services through the internet. Now I understand more about containers, databases, deployment, and how different services can work together. This activity also helped me understand why Docker Compose is useful when deploying multiple containers.
