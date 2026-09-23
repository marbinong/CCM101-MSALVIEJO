# Storage Types Research

## Comparison of Cloud Storage Types

| Storage Type | Description | Primary Use Case | Cloud Provider Example |
|---|---|---|---|
| **Block Storage** | Stores data in fixed-size blocks that can be attached to a virtual machine like a hard drive. | Best for operating systems, databases, and applications that need fast storage. | AWS EBS |
| **File Storage** | Stores data as files organized into folders and directories. Multiple users or systems can access the same files. | Best for shared files, documents, and applications that need a shared file system. | AWS EFS |
| **Object Storage** | Stores data as objects together with metadata and a unique identifier. It is designed for large amounts of unstructured data. | Best for photos, videos, backups, documents, and other large collections of files. | AWS S3 |

## Why Object Storage Is Best for User-Uploaded Images

Object Storage is the best choice for storing millions of user-uploaded images because it is designed to handle large amounts of unstructured data. It can store many files efficiently and allows applications to access images through a unique object identifier, making it suitable for a photo-sharing application.
