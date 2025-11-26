## Amazon Storage Services

<img width="663" height="282" alt="type-of-storage-1" src="https://github.com/user-attachments/assets/01485c29-4d7d-4ca5-affb-a7a6727ebdfe" />

Amazon offers three different storage services with differet use cases. Amazon Simple Storage Service commonly known as S3 is used for object storage. Objects are any files that can be stored on S3 itself, it's the actual data. Amazon S3 uses buckets (similar to directories) where objects can be stored. Object keys are unique identifiers for objects within a bucket. S3 is highly available, durable and secure service. Amazon S3 has seven different storage classes, each differentiated by their use cases and access frequency. Different classes will have different costs. S3 is a provisioned regionally upon setup and offers versioning , object locking, static website hosting and event notification features.

<img width="1884" height="603" alt="24_S3_intelligent_tiering_1_c2c89726c2" src="https://github.com/user-attachments/assets/52344f00-ee9a-4c23-83ee-fc61725627d1" />

Amazon Elastic File System is cloud based network file system storage service for compute instances or own-premises servers. It is designed primarily for Linux workloads and supports NFS and uses tags. The benefits of EFS is high availability, dynamic elasticity and fully managed servcices offering a good value proposition for AWS customers. EFS is used for media workflows, database backups, big data analytics and home directories among other uses.

<img width="935" height="530" alt="s3-vs-ebs-vs-efs" src="https://github.com/user-attachments/assets/153a23c2-827e-431f-87ad-77c0ec8373f0" />


Amazon Elastic Block Service provides persistent storage for Amazon EC2 instances. Persistent storage is similar to a hard-drive on your computer.  EBS features backshots, encryption and multiple volumes. EBS volumes can be used as boot volumes and primary storage of EC2 instances and snapshots are a backups of the EBS volumes. Volumes could be HDD or SSD, and there are different classes for different use casses. 


<img width="980" height="494" alt="1_x7Hjy4qA5AtWZTqYa0CgkQ" src="https://github.com/user-attachments/assets/936923cc-1f96-4d5a-b68e-9d67369c2737" />

