- [[Deployment - Summary]]
- Helps you manage your **[[EC2 - Elastic Compute Cloud]] and On-Premises** systema at scale
- Another **hybrid** AWS service
- Most important features are:
	- Patching automation for enhanced compliance
	- Run commands across an entire fleet of servers
	- Store parameter configuration with the [[Systems Manager parameter Store]]
- Works for Linux, Windows, MacOS, and Raspberry

How Systems Manager works
- We need to install the SSM agent onto the systems we control
- Installed by default on Amazon Linux AMI & some Ubuntu AMI
- Thanks to the SSM agent, we can **run commands, patch & configure our servers**
- If instance can't be controlled with SSM, it's probably an issue with SSM agent

![[Pasted image 20240523112017.png]]
SSM Session Manager
- Allows you to start a secure shell on your EC2 and on-premises servers
- **No SSH access, bastion hosts, or SSH keys needed**
- No port 22 needed
- Supports Linux, macOS, and Windows

![[Pasted image 20240523112516.png]]
