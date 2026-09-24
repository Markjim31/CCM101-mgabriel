# Mission Reflection

Object storage is better suited for storing millions of photos because it is designed for large amounts of unstructured data. Photos can be stored as individual objects with their associated metadata. This makes object storage appropriate for applications that need to store and access large numbers of images. Traditional block storage works more like a virtual hard drive and is useful for systems that require direct disk access.

Docker made it easier to deploy the MinIO storage server because the application could run inside a container without requiring a long manual installation process. The Docker command configured the ports, administrator credentials, and storage server. This made the deployment process more organized and repeatable.

A bucket is a logical storage container used to organize objects in an object storage system. In this laboratory, I created a bucket named `client-photos` for the sample files representing user-uploaded photos.

Large enterprise companies can reduce the risk of data loss by using redundant storage systems, backups, replication, and distributed infrastructure. These methods can help keep data available even when physical hardware fails.

My confidence in navigating the Linux command line is growing because I have become more comfortable entering commands and checking their results. In this laboratory, I used Docker commands to deploy and verify a storage service. I also learned how a containerized application can be accessed through specific ports and managed through a web interface. Creating the bucket and uploading a file helped me understand how object storage works in a practical environment. Overall, this activity helped me connect Docker skills from the previous laboratory with cloud storage concepts.
