# Mission Reflection

Writing a `docker-compose.yml` file makes a cloud engineer's job easier because it allows multiple containers to be configured and deployed using one file. In this laboratory, I used Docker Compose to deploy Nextcloud and MariaDB together instead of manually typing separate commands for each container. This made the deployment more organized and easier to repeat.

I also experienced why YAML indentation is important. When creating the Compose file, I encountered problems with the formatting and indentation. YAML depends on spaces to identify the structure of the configuration. Using incorrect indentation or a Tab can cause errors and prevent Docker Compose from reading the file correctly. This taught me to be more careful when creating configuration files.

We used environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, `MYSQL_USER`, and `MYSQL_HOST` because they provide the information needed for Nextcloud to connect to the MariaDB database. In my deployment, `MYSQL_HOST=database` allowed the Nextcloud application to find the MariaDB container through the service name. This showed me how different containers can communicate with each other.

It was satisfying to see Nextcloud running after creating the configuration and starting the containers. I was able to access the Nextcloud setup page through port 8080 and verify that the application was working. Even though I encountered some configuration issues, I was able to correct them and complete the deployment.

Since Mission 1, my understanding of Cloud Computing has developed from learning about cloud platforms such as AWS, Azure, and GCP to actually working with containers and cloud deployment tools. I now understand that cloud computing is not only about cloud providers but also about how applications, databases, networking, and infrastructure can work together. This laboratory gave me more practical experience in deploying and documenting a cloud-based application.
