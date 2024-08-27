- AMI are a customization of an [[EC2 - Elastic Compute Cloud]] instance
	- you add your own software, configuration, os, monitoring
	- Faster boot / configuration time because all your software is pre-packaged
- AMI are built for a specific region (and can be copied across regions)
- You can launch EC2 instances from:
	- A Public AMI: AWS provided
	- Your own AMI: you make and maintain them yourself
	- an AWS Marketplace AMI: an AMI someone else made

AMI Process (from an EC2 instance)
- Start an EC2 instance and customize it
- Stop the instance (for data integrity)
- Build an AMI
	- this will create EBS snapshots
- Launch instances from other AMIs

EC2 Image Builder
- Used to automate the creation of Virtual Machines or container images
- Automate the creation, maintain, validate and test EC2 AMIs
- Can be run on a schedule
- Free service (only pay for the underlying resources)