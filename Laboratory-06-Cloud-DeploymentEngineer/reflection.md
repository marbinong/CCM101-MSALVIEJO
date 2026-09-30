# Mission Reflection

Writing a `docker-compose.yml` file makes a cloud engineer's job easier because it allows multiple containers to be configured and deployed using one file. Instead of typing many commands manually, the configuration can be saved and reused. This also helps reduce mistakes and makes the deployment process more organized.

An indentation error in a YAML file can cause problems when Docker Compose reads the configuration. YAML depends on proper spacing and indentation to understand the structure of the file. Using a Tab instead of spaces or placing a line at the wrong level may result in an error, and the containers may not start correctly.

We used environment variables such as `MYSQL_PASSWORD`, `MYSQL_DATABASE`, and `MYSQL_USER` to provide the required database configuration to the containers. These variables allow the Nextcloud application to know which database information and credentials it should use. They also make the configuration easier to understand and modify.

Deploying Nextcloud in just a few minutes was a good experience because it showed how cloud technologies can simplify application deployment. Instead of manually installing and configuring every component, Docker Compose handled the containers based on the configuration file. Seeing the Nextcloud setup page in the browser also helped me understand how containers can provide actual services that users can access.

Since Mission 1, my understanding of Cloud Computing has improved. I started by learning basic Linux commands, cloud infrastructure, and system information. In this mission, I was able to apply those skills to container deployment and Infrastructure as Code. I now have a better understanding of how different components can work together as one cloud application.

