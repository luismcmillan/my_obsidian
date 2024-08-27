- [[Databases & Analytics Summary]]
- RDS stands for Relational Database Service
- it allows you to create databases in the cloud that are managed by AWS
	- Prostgres
	- MySCL
	- MariaDB
	- Oracle
	- Microsoft SWL Server
	- IBM DB2
	- Aurora

**Advantage over using RDS** versus deploying DB on [[EC2 - Elastic Compute Cloud]]

- RDS is a managed service:
	- Automated provisioning, OS patching
	- Continuous backups and restore to specific timestamp
	- Monitoring dashboards
	- Read replicas for improved read performance
	- Multi AZ setup for DR (Disaster Recovery)
	- Maintenance windows for upgrades
	- Scaling capability (vertically horizontal)
	- storage backed by [[EBS (Elastic Block Store) Volume]]
- **BUT you can't SSH into your instances**
