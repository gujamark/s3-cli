# S3 CLI program

# Description
This is a CLI implementation of AWS S3 service, which allows to list buckets, create bucket, download/upload files, assign policies, etc.

### Dependencies
- botocore
- magic

### Avaliable Flags

| Short | Long | Description |
|-----|-----|----|
| -lb | --list_buckets: |  List already created buckets. | 
| -cb | --create_bucket: |  Flag to create a bucket. | 
| -bn | --bucket_name: |  Pass the name of the bucket. | 
| -bc | --bucket_check: |  Check if the bucket already exists. | 
| -region | --region: |  Region variable. | 
| -db | --delete_bucket: |  Flag to delete a bucket. | 
| -be | --bucket_exists: |  Flag to check if a bucket exists. | 
| -rp | --read_policy: |  Flag to read the bucket policy. | 
| -arp | --assign_read_policy: |  Flag to assign a read bucket policy. | 
| -amp | --assign_missing_policy: |  Flag to assign a missing bucket policy. | 
| -du | --download_upload: |  Download and upload to the bucket. | 
| -ol | --object_link: |  Link to download and upload to the bucket. | 
| -lo | --list_objects: |  List bucket objects. | 
| -ben | --bucket_encryption: |  Bucket object encryption. | 
| -rben | --read_bucket_encryption: |  List bucket object. | 
| -uf | --upload_file: |  Upload a small file to the bucket. | 
| -mpu | --multipart_upload: |  Multipart file upload. | 
| -file | --file: |  File which will be uploaded to the bucket. | 
| -lce | --lifecycle_expiration_days: |  After how many days objects will be deleted. | 
| -del | --delete_object: |  Delete the object from the bucket. | 

## Examples

### List Buckets

```
python main.py --list_buckets
```

### Create Bucket
```
python main.py --bucket_name my-new-bucket --create_bucket --region us-west-2
```

### Download and Upload to Bucket
```
python main.py --bucket_name my-bucket
```
