- [[EC2 - Elastic Compute Cloud]]
- Network drive attached to 
	- uses network to communicate
	- can be detached from EC2 to another one quickly
- allows persisting data even after EC2 termination
- can only be **mounted to one instance at a time**
- bound to specific AZ
- get billed for provisioned capacity
- you can increase capacity over time
- Delete on Termination attribute
	- by default root EBS is deleted (attribute enabled)
	- by default, any other attached EBS volume is not deleted (attribute disabled)

[[EBS Snapshots]]