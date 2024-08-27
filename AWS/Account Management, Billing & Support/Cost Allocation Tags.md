- [[Account Best Practices - Summary]]
- Use cost allocation tags to track your AWS costs on a detailed level
- AWS generated tags
	- Automatically applied to the resource you create
	- Starts with Prefix aws:
- User-defined tags
	- Defined by the user
	- Starts with Prefix user:

Tagging and Resource Groups
- Tags are used for organizing resources
	- EC2: instances, images, load balancers, security groups
	- RDS, VPC
	- Resources created by CloudFormation are all tagged the same way
- Free naming, common tage are: Name,Environment
- Tags can be used to create **Resource Groups**
	- Create, maintain, and view a collection of resources that share common tags
	- Manage these tags using the Tag Editor