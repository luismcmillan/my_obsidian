- [[Well Architected Framework]]
- Ability of a system to recover from infrastructure or service disruptions, dynamically acquire computing resources to meet demand, and mitigate disruptions such as misconfigurations or transient network issues
- Design Principles
	- **Test recovery procedures** - Use automation to simulate different failures or to recreate scenarios that led to failures before
	- **Automatically recover from failure** - Anticipate and remediate failures before they occur
	- **Scale horizontally to increase aggregate system availability** - Distribute requests across multliple, smaller resources to ensure that they don't share a common point of failure
	- **Stop guessing capacity** - Maintain the optimal level to satisfy demand without over or under provisioning - Use auto Scaling
	- **Manage change in automation** - Use automation to make changes to infrastructure
![[Pasted image 20240525224331.png]]