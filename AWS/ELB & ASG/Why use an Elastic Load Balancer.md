- [[EC2 - Elastic Compute Cloud]]
- An ELB is **managed load balancer**
	- AWS guarantees that it will be working
	- Distributes traffic across backend EC2 instances, can be Multi-AZ
	- AWS takes care of upgrades, maintenance, high availability
	- AWS provides only a few configuration knobs
- it costs less to setup own load balancer but it will be a lot more effort on your end
- 4 kinds of load balancers
	- Application Load Balancer (HTTP / HTTPS only) - Layer 7
	- Network Load Balancer (ultra-high performance, allows for TCP) - Layer 4
	- Gateway Load Balancer - Layer 3
	- Classic Load Balancer (retired) - Layer 4 & 7
![[Pasted image 20240522094827.png]]

[[Auto Scaling Group]]