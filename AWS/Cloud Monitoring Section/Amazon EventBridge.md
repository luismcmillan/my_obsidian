- [[Lambda]]
- Schedule: Cron jobs (scheduled scripts)
![[Pasted image 20240524091337.png]]
- Event Pattern: Event rules to react to a service doing something
![[Pasted image 20240524091421.png]]
- Trigger Lambda functions, send SQS/SNS messages

Rules:
![[Pasted image 20240524091703.png]]
Eventtypes:
![[Pasted image 20240524094034.png]]
- Schema Registry: model event schema
- You can **archive events** (all/filter) sent to an event bus (indefinitely or set period)
- Ability to **replay archived events**
-