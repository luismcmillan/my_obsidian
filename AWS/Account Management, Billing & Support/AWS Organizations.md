- [[Account Best Practices - Summary]]
- Global service
- Allows to manage **multiple AWS accounts**
- The main account is the master account
- Cost Benefits
	- Consolidated Billing across all accounts - single payment method
	- Pricing benefits from **aggregated usage**
	- Pooling of Reserved [[EC2 - Elastic Compute Cloud]] instances for optimal savings
- API is available to automate AWS account creation
- **Restrict account privileges using Control Policies (SCP)

Multi Account Strategies
- Create accounts per **department**, per cost center, per dev / test / prod, based on regulatory restrictions (using [[Service Control Policies (SCP)]]), for better resource isolation (ex:[[VPC Summary]]) to have separate per-account service limits, isolated account for logging
![[Pasted image 20240524172025.png]]
![[Pasted image 20240524172115.png]]

- Multi Account vs One Account MultiVPC
- Use tagging standards for billing purposes
- Enable [[AWS CloudTrail]] on all accounts, send logs and to central [[Amazon S3]] account
- Send [[CloudWatch]] Logs to central logging account