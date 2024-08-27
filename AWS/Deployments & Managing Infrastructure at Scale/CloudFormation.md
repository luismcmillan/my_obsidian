- [[Deployment - Summary]]
- CloudFormation is a declarative way of outlining your AWS Infrastructure, for any resources
- **free to use**
- For example, within a CloudFormation template, you say
	- I want a security group
	- I want two EC2 instances using security group

- Then CloudFormation creates those for you , in the **right order**, with the **exact configuration** that you specify

- **Infrastructure as code**
	- No resources are manually created, which is excellent for control
	- Changes to the infrastructure are reviewed through code
	- Productivity
		- Ability to destroy and re-create an infrastructure on the cloud on the fly
	- Don't re-invent the wheel
		- Leverage existing templates on the web!