- CloudWatch provides metrics for every services in AWS
- **Metric** is a variable to monitor
- Metrics have **timestamps**
![[Pasted image 20240524085440.png]]
Important Metrics:
- [[EC2 - Elastic Compute Cloud]] instances: CPU Utilization, Status Checks, Network (not RAM)
	- Default metrics every 5 minutes
- EBS volumes: Disk Read/Writes
- S3 buckets: BucketSizeBytes, NumberOfObjects,AllRequests
- Billing; Total Estimated Charge (only in us-east-1)
- Service Limits: how much you've been using service API
- [[Amazon CloudWatch Alarms]]