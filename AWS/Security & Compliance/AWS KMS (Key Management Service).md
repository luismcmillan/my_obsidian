- Anytime you hear "encryption" for an AWS service , its most likely KMS
- **KMS = AWS manages the encryption keys for us**
- Encryption Opt-in:
	- [[EBS (Elastic Block Store) Volume]]: encrypt volumes
	- [[Amazon S3]] buckets: Server-side encryption of objects
	- [[Redshift]] database: encryption of data
	- [[Amazon RDS]] database: encryption of data
	- [[EFS - Elastic File System]] drives; encryption of data
	
- Encryption Automatically enables:
	- [[AWS CloudTrail]] Logs
	- [[Amazon S3]] Glacier
	- [[AWS Storage Gateway]]

Typed of KMS Keys
- Customer Managed Key:
	- Create, manage and used by the customer, can enable or disable
	- Possibility of rotation policy (new key generated every year, old key preserved)
	- Possibility to bring-your own-key
- AWS Managed Key:
	- Created, managed and used on the customer's behalf by AWS
	- Used by AWS services (AWS/s3, aws/ebs, aws/redshift)
- AWS Owned Key;
	- Collection of CMKs that an AWS service owns and manages to use in multiple accounts
	- AWS can use those to protect resources in your account (but can't view the keys)
- [[CloudHSM]] keys (custom keystore):
	- Keys generated from your own CloudHSM hardware device
	- Cryptographic operations are performed within the CloudHSM cluster