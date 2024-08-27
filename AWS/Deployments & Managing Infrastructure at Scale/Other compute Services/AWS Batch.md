- A "batch" job is a job with a start and an end (opposed to continuous)
- **Filly managed** batch processing at any scale
- Batch will dynamically launch [[EC2 - Elastic Compute Cloud]] instances or Spot Instances
- Batch jobs are defined as [[Docker]] images and run on [[ECS - Elastic Container Service]] 

![[Pasted image 20240523091956.png]]
- **no time limit**
- Any runtime as long as packaged as a [[Docker]] image
- Rely on [[EBS (Elastic Block Store) Volume]]
- Relies on EC2