- [[Monitoring Summary]]
- Debugging in Production, the good old way:
	- test locally
	- Add log statements everywhere
	- Re-deploy in production
- Log formats differ across applications and log analysis is hard
- Debugging: one big monolith "easy", **distributed services "hard"**
- No common views of your entire architecture

- **Enter.. AWS X-Ray**
![[Pasted image 20240524095401.png]]
advantages:
- Trouvleshooting performance (nottlenecks)
- Understand dependencies in a microservice architecture
- Pinpoint service issues
- Review request behavior
- Find errors and exceptions
- Are we meeting time SLA (Service Level Agreement)
- Where I am throttled
- Identify usere that are impacted