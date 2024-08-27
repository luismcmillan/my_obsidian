- [[VPC Summary]]
- Site to Site VPN
	- Connect an on-premises VPN to AWS
		- On-premises must use a **Customer Gateway (CGW)
		- AWS: must use a **Virtual Private Gateway (VGW)**
		![[Pasted image 20240524120116.png]]
	- The connection is automatically encrypted (IPSec)
	- Goes over the **public internet**
![[Pasted image 20240524115616.png]]
- Direct Connect (DX)
	- Establish a physical connection between on-premises and AWS
	- The connection is private, secure and fast
	- Goes over the **private network**
	- Takes at least a month to establish