-[[Messages]]
![[Pasted image 20240523192024.png]]
- Fully managed service (serverless) use to **decouple** applications
- Scales from 1 message per second to 10000
- Default retention of messages: 4 days, maximum of 14 days
- No limit to how many messages can be in the queue
- **Messages are deleted after they're read by consumers
- Consumers share the work to read messages & scale horizontally
![[Pasted image 20240523192431.png]]

![[Pasted image 20240523192524.png]]
