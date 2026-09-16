# Mission Reflection

This laboratory activity helped me understand how containerization is different from using a Virtual Machine. Installing an operating system on a Virtual Machine normally takes more time because the VM needs to create virtual hardware and boot a complete operating system. In comparison, a Docker container can start within seconds because it shares the host operating system kernel. The setup process is also simpler when the required Docker image is already available.

Port mapping such as `-p 8080:80` is necessary because the Nginx web server is running inside the container on port 80. The port mapping connects port 8080 of the host machine to port 80 inside the container. This allows users or applications on the host machine to access the web server through `http://localhost:8080`. Without port mapping, the web server may not be directly accessible from the host.

When the `docker rm` command is used, the container itself is permanently removed. Any data stored only inside the writable layer of that container is also removed. However, data stored using Docker volumes or other external storage can remain after the container is deleted. This shows why persistent data should be stored separately when needed.

Containerization can also change how software developers and IT operations teams work together. Developers can package an application and its dependencies into a container, making it easier for operations teams to run the same application in different environments. This supports DevOps practices by making application deployment more consistent and easier to automate.

My GitHub portfolio is also becoming more organized as I complete each laboratory activity. Instead of keeping only separate screenshots or notes, I am learning to document commands, explanations, results, and reflections using Markdown. Laboratory 04 adds Docker and containerization to my portfolio and shows my progress in learning cloud computing and cloud-native technologies.
