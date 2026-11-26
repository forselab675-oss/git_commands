# AWS COMMANDS

## 1. Install AWS CLI (Ubuntu)

sudo apt update

# Updates package lists

sudo apt install unzip curl -y

# Installs required utilities

curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"

# Downloads AWS CLI

unzip awscliv2.zip

# Extracts the downloaded file

sudo ./aws/install

# Installs AWS CLI

## 2. Check AWS CLI

aws --version

# Checks AWS CLI version

## 3. Configure AWS

aws configure

# Configures AWS credentials and default region

# Enter:
# AWS Access Key ID
# AWS Secret Access Key
# Default region name (example: ap-south-1)
# Default output format (example: json)

## 4. Check Identity

aws sts get-caller-identity

# Displays the configured AWS account identity

## 5. List S3 Buckets

aws s3 ls

# Lists S3 buckets

## 6. Create S3 Bucket

aws s3 mb s3://my-unique-bucket-name --region ap-south-1

# Creates an S3 bucket
# Bucket name must be globally unique

## 7. Upload File to S3

aws s3 cp file.txt s3://my-unique-bucket-name/

# Uploads file.txt to the bucket

## 8. Download File from S3

aws s3 cp s3://my-unique-bucket-name/file.txt .

# Downloads file.txt to current folder

## 9. List EC2 Instances

aws ec2 describe-instances --region ap-south-1

# Displays EC2 instance details

## 10. List EC2 Instance IDs and States

aws ec2 describe-instances --region ap-south-1 --query "Reservations[*].Instances[*].[InstanceId,State.Name]" --output table

# Displays instance IDs and their states

## 11. Delete S3 Bucket

aws s3 rb s3://my-unique-bucket-name --force

# Deletes bucket and its contents
