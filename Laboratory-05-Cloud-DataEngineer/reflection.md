
# Mission 5 Reflection

This laboratory activity helped me understand why object storage is useful for applications that handle large amounts of data, especially photos. Object storage is better suited for storing millions of photos because it is designed for unstructured data such as images, videos, and backups. Instead of treating every file like a part of a traditional hard drive, object storage stores each file as an object with metadata and a unique identifier. This makes it easier for applications to manage and access a very large number of files.

Using Docker also made deploying the MinIO server easier. Instead of manually installing and configuring many components, I only needed to run one Docker command with the required ports, image, and environment variables. Docker automatically created the container and allowed MinIO to run in an isolated environment. This made the deployment process faster and easier to reproduce.

A bucket in cloud storage is a container used to organize and store objects or files. In this activity, I created a bucket named `client-photos` where I uploaded a sample file. The bucket helped demonstrate how files can be organized in an object storage system.

Large enterprise companies can protect their object storage data from physical server failures by using multiple copies of data, redundancy, backups, and replication across different servers or locations. These methods help ensure that data can still be recovered even when a physical server or storage device fails.

My confidence in using the Linux command line is also improving. At first, commands can be difficult to understand, but practicing Docker commands, checking containers, and working with files has made me more comfortable. I learned that carefully reading each command and understanding its options is important. This activity also showed me how Linux, Docker, and cloud storage can work together to create a practical cloud environment.
