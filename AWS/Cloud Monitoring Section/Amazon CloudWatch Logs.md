- CloudWatch Logs can collect from
	- [[AWS Elastic Beanstalk]]: collection of logs from application
	- [[ECS - Elastic Container Service]]: collection from containers
	- [[Lambda]]: collection from function logs
	- [[AWS CloudTrail]]: based on filter
	- **Cloudwatch log agents: on [[EC2 - Elastic Compute Cloud]] machines or on-premises servers
	- [[Amazon Route 53]]: Log DNS queries

- Enables **real-time monitoring of logs**

CloudWatch Logs for EC2
- By Default, no logs from your EC2 instance will go to CloudWatch
- You need to run a CloudWatch agent on EC2 to push the log files you want
- Make sure [[Permissions]] are correct
- CloudWatch log agent can be setup on-premises too
![[Pasted image 20240524091012.png]]
