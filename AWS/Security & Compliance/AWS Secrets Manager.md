- Capability to force **rotation of secrets** every X days
- Automate generation of secrets on rotation (uses [[Lambda]])
- Integration with [[Amazon RDS]] (MySQL, PostgreSQL, Aurora)
- Secrets are encrypted using [[AWS KMS (Key Management Service)]]
- Mostly meant for RDS integration
- anytime you see a secret to be managing in RDS and to be rotated, its **Secrets Manager**