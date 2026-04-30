# IAM Lab — Setup Steps

## Step 1: Create IAM User
- Created user: test-user

## Step 2: Create IAM Group
- Created group: test-group
- Attached S3 read-only policy to group

## Step 3: Attach Direct User Policy
- Attached custom policy allowing S3 full access

## Step 4: Add Conflicting Policy
- Attached explicit deny policy for s3:DeleteObject

## Step 5: Add User to Group
- User now has:
  - Group policy
  - User policy
  - Explicit deny policy

## Step 6: Test Access
- Attempted:
  - S3 list
  - S3 upload
  - S3 delete
