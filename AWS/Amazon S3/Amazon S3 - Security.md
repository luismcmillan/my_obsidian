- [[Amazon S3]]
- User-Based
	- IAM Policies - which API calld should be allowed for specific user from IAM
- Resource-Based
	- Bucket Policies - bucket wide rules from the S3 console - allows cross account
	- Object Access Control List (ACL) - finer grain
	- Bucket Access Control List (ACL) - less common

- Note: an IAM principal can access an S3 object if
	- user IAM permissuins ALLOW it OR the resource policy ALLOWS it
	- AND there is no explicit DENY

- Encryption: encrypt objects in Amazon S3 using encryption keys