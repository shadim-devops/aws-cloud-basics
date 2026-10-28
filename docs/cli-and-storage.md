# AWS CLI and S3 Operations

## Objective

Practice basic AWS CLI commands for storage management and resource discovery.

## Amazon S3

Created an S3 bucket and tested file upload and download.

Representative commands:

```bash
# List buckets
aws s3 ls

# Upload a local file
aws s3 cp ./example.txt s3://<your-bucket-name>/example.txt

# Download the file
aws s3 cp s3://<your-bucket-name>/example.txt ./downloaded-example.txt
```

Bucket creation requires a globally unique name and Region-specific options; follow the current AWS CLI documentation for the target Region.

## EC2 Resource Inspection

Listed available Amazon Machine Images (AMIs):

```bash
aws ec2 describe-images --owners amazon --region <aws-region> --query 'Images[].{Id:ImageId,Name:Name}' --output table
```

Listed security groups:

```bash
aws ec2 describe-security-groups --region <aws-region>
```

## IAM Inspection

Listed IAM users and inspected user details:

```bash
aws iam list-users
aws iam get-user --user-name <user-name>
```

## Result

Successfully performed S3 file transfers and inspected AWS resources and IAM users through the AWS CLI.

> Note: The commands above are representative examples. Resource names, account IDs, and Region values are placeholders rather than claims about the original environment.
