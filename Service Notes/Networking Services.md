## Networking Services

![1716442749895](https://github.com/user-attachments/assets/5837dfd7-5e81-4ca0-a765-1afae77fcb50)

AWS offers Virtual Private Cloud (VPC) for it's clients to create an isolated network within their AWS environment. It allows control over your environment and resources giving clients the control of who has access to what, how traffic and data flows and which resources are connected to what. It gives clients the ability to design and customise their AWS environment according to their business and organizational needs.

A VPC contains a subnet, route table ,Internet gateway, NAT gateway, security group and Network Access List (Network ACL). A subnet is a smaller partition of a network, which can either be private or public. A subnet allows for better network performance and to better isolate resources. Public subntes are suitable for resources that can be accessed through the internet such as web servers and private subnets are suitable for resources that shouldn't be accessed through the internet such as a database. Route tables are sets of rules known as routes that determine where traffic is directed and can determine the target and destination.

Internet gateways allows resources in public subnets to be accessed through the internet via IPv4 or IPV6 addresses. NAT Gateways or NAT Instances are similar to Internet Gateways but for private subnets. They allow resources in the private subnets to access the internet whilst remaining private. A security group is a virtual firewall at the instance level and controls inbound and outbound traffic through inbound and outbound rules. Networks ACL's are similar to subnets but act on the subnet level rather than the instance level. They also have allow and deny rules which control traffic flow.

<img width="1369" height="480" alt="083e6df5-5419-40c5-931b-78520f668fbf" src="https://github.com/user-attachments/assets/cc48aa8c-60d9-45d0-84e8-0fbb84afc9f8" />

Additional features of VPC's are VPC's flow logs, VPC Peering ,VPC Endpoints and AWS Virtual Private Network. A VPC flow log is a log file of the traffic flow through the virtual private cloud. VPC Peering enables two virtual private clouds to establish a network connection privately using IPV4 or IPV6 addresses. VPC Endpoints allows clients to connect their VPC Endpoint to other supported AWS services or VPC Endpoint services. A Virtual Private Network or VPN allows for a private connection between your laptop at home to AWS, on premises servers to AWS or remote devices to AWS.AWS VPN may either be site-to-site VPN or AWS Client VPN. A site-to-site VPN allows to connection between on premises environment to AWS and the client VPN allows connection between a remote employee to AWS.

Amazon PrivateLink allows a connection between on premises environment to AWS without a connection through the internet. AWS TransitGateway allows for simple management of multiple VPC's and  on premises environment.

**Use cases**

* Create hybrid connections (VPC)
* Stream live and on-demand videos (CloudFront)
* Manage large datasets (DirectConnect)
* Consistent high performance
* Broadest gloabal coverage
* Highest network availability

**Benefits**

* Improve Security
* Improved application perfromance
* Automatic scaling
* Reduce latency
* Monitor in real time
  
