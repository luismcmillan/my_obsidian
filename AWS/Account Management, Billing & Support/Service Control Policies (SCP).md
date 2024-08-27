- [[Account Best Practices - Summary]]
- Whitelist or blacklist [[IAM]] actions
- Applied at the OU or Account level
- Does not apply to the Master Account
- SCP is applied to all the **Users and Roles** pf the Account, including Root
- The SCP does not affect service-linked roles
	- Service-linked roles enable other AWS services to integrate with AWS Organizations and can't be restricted by SCPs
- SCP must have an explicit Allow
![[Pasted image 20240524180035.png]]
