- [[Amazon S3]]
- Amazon S3 Standard - General Purpose
	- 99.99% Availability
	- Used for frequently accessed data
	- low latency and high throughput
- Infrequent Access:
	- For data that is less frequently accessed, but required rapid access when needed
	- lower cost than S3 Standard
	- Amazon S3 Standard-infrequent Access (IA)
		- 99,9% Availability
	- Amazon S3 One Zone-Infrequent Access
		- 99.5% Availibility
		- 99.999999999% durability
[[AWS Snow Family]]:
- Amazon S3 Glacier Storage Classes
	- **low-cost** object storage meant for archiving / backup
	- Pricing: price for storage + object retieval cost
	- Amazon S3 Glacier Instant Retrieval
		- Millisecond retrieval
		- Minimum storage duration of 90 days
	- Amazon S3 Glacier Flexible Retrieval
		- Expedited (1-5 minutes), Standard (3-5 hours), Bulk (5 -12 hours) - free
	- Amazon S3 Glacier Deep Archive
		- Standard (12 hours), Bulk (48 hours)
Amazon S3 Intelligent Tiering
	- Small monthly monitoring and auto-tiering fee
	- Moves objects automatically between Access Tiers based on usage
	- There are no retrieval charges in S3 Intelligent-Tiering

- Can move between classes manually or using S3 Lifecycle configurations

**Encryption**
- Server-Side Encryption (Default)

**Durability**:
- High durability 99,999999999 % of objects across multiple AZ
- same for all storage classes

**Availability**:
- Measures how readily available a service is
- Varies depending on storage class