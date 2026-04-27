# IAM Lab 4 — Steps

## Step 1: Create IAM Role
- Created role for EC2 service
- Selected EC2 as trusted entity

## Step 2: Attach Policy to Role
- Attached `AmazonS3ReadOnlyAccess` policy

## Step 3: Launch EC2 Instance
- Launched EC2 instance
- Attached IAM role during setup

## Step 4: Access EC2
- Connected to EC2 via SSH

## Step 5: Test S3 Access from EC2
- Ran command to list S3 buckets
- Successfully accessed S3 without using access keys

## Step 6: Verify No Access Keys Used
- Confirmed no access keys were stored on the instance
