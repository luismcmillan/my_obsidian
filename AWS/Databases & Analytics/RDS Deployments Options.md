- [[Databases & Analytics Summary]]
- Read Replicas:
	- Scale the read workload of your DB
	- Can create up to 15 Read Replicas
	- Data is only written to the main DB

- Multi-AZ:
	- Failover in case of AZ outage (high availability)
	- Data is only read/written to the main database
	- Can only have 1 other AZ as failover

- Multi-Region
	- Disaster recovery in case of region issue
	- Local performance for glabal reads
	- Replication cost