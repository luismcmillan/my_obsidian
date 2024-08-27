[Boss]
- **EC2 = Infrastructure as a Service**
- mainly consists in capability of
	- Renting virtual machines (EC2)
	- Storing data on virtual drives[[EBS (Elastic Block Store) Volume]]
	- Distributing load across machines (ELB)
	- Scaling the services using an auto-scaling group (ASG)
- EC" sizing & configuration options
	- Operating System (OS): Linux, Windows or Mac Os
	- compute power & cores (CPU)
	- how much random-access memory (RAM)
	- how much storage
		- Network-attached (EBS & EFS)
		- hardware (EC2 Instance Store)
	- Network card: speed of the card, Public IP address
	- Firewall rules: security group
	- **Bootstrap script** (configure at first launch): EC2 User Data
		- means launching commands when machine starts
		- script only run once at the instance first start
		- EC2 user data is used to automate boot tasks such as:
			- Installing updates
			- installing software
			- Downloading common files from the internet
			- Anything you can think of
		- EC2 User Data Script runt with root user (**sudo**)
[[EC2 Instance Types - Overview]]
[[Security Groups]]
[[Classic Ports to know]]
[[EC2 Instance Connect]]
[[EC2 Instances Purchasing Options]]
[[EC2 Shared Responsibility Model]]

[[AMI (Amazon Machine Image)]]
[[EC2 Instance Store]]
[[Amazon FSx]]
[[EFS - Elastic File System]]
[[Why use an Elastic Load Balancer]]