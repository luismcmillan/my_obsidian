- [[Amazon S3]]
- You can version your files in Amazon S3
- it is enables at the bucket level
- Same key overwrite will change the 'version': 1,2,3
- It is best practice to version your bucket
	- Protect against unintended deletes (ability to restore a version)
	- Easy roll back to previous version
- Notes:
	- Any file is not versioned prior to enabling versioning will have version "null"
	- Suspending versioning does not delete the previous versions