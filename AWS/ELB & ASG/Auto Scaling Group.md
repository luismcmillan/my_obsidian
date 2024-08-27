- In real-life, the load on your websites and application can change
- In cloud you can create and get rid of servers very quickly
- **Goal of ASG**
	- Scale out (add [[EC2 - Elastic Compute Cloud]] instances) to match an increased load
	- Scale in (remove EC2 instances) to match a decreased load
	- Ensure we have a minimum and maximum number of machines running
	- automatically register new instances to a load balancer
	- Replace unhealthy instances
- Cost Savings: only run at an optimal capacity (principle of the cloud)
[[Scaling Groups - Scaling Strategies]]