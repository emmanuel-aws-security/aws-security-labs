# IAM Lab 6 — Steps

## Step 1: Create IAM User
- Created test IAM user

## Step 2: Attach Allow Policy
- Attached policy allowing S3 access:
  - s3:ListBucket
  - s3:GetObject

## Step 3: Test Access
- Confirmed user can access S3 resources

## Step 4: Attach Deny Policy
- Attached explicit deny policy for S3 actions

## Step 5: Re-Test Access
- Attempted S3 access again
- Access was denied

## Step 6: Observe Result
- Despite having allow permissions, access was blocked due to explicit deny
