- Automated Security Assessments
![[Pasted image 20240524150500.png]]
- For [[EC2 - Elastic Compute Cloud]] instances
	- Leveraging the [[AWS Systems Manager (SSM)]] agent
	- Analyze against unintended network accessibility
	- Analyze the running OS against known vulnerabilities
- For Container Images push to [[ECR - Elastic Container Registry]]
	- Assessment of Container Images as they are pushed
- For [[Lambda]] Functions
	- Identifies software vulnerabilities in function code and package dependencies
	- Assessment of functions as they are deployed

- Reporting & integration with AWS Security Hub
- Send findings to [[Amazon EventBridge]]

- **A risk score is associated with all vulnerabilities for prioritization**