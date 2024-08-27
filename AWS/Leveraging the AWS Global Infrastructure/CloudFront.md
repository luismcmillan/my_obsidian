
- [[Amazon S3 - Buckets]]
- Content Delivery Network (CDN)
- **Improves read performance, content is cached at the edge**
- DDoS protection (because worldwide), integration with Shield, AWS Web Application Firewall

Origins:
- S3 bucket
	- For distributing files and caching them at the edge
	- Enhanced security with CloudFront **Origin access Control (OAC)**
	- OAC is replacing Origin Access Identity (OAI)
	- CloudFront can be used as an ingress (to upload files to S3)
- Custom Origin (HTTP)
	- Application Load Balancer
	- EC2 instance
	- S3 website (must first enable the bucket as a static website)

CloudFront at a high level:
![[Pasted image 20240523151341.png]]

S3 as an Origin:
![[Pasted image 20240523151656.png]]

- CloudFront
	- Global Edge network
	- Files are cached for a TTL
	- **Great for static content that must be available everywhere**

- S3 Cross Region Replication
	- Must be setup for each region you want replication to happen
	- Files are updated in near real-time
	- Read only
	- **Great for dynamic content that needs to be available at low-latency in few regions**

[[CloudFront - Pricing Storage]]