# IAM Lab 3 — Steps

## Step 1: Review Policy Structure
- Opened IAM policy JSON
- Observed key elements:
  - Effect
  - Action
  - Resource

## Step 2: Attach Over-Permissioned Policy
- Attached `AdministratorAccess` to test user

## Step 3: Test Full Access
- Accessed S3 (list, upload, delete)
- Launched EC2 instance
- Confirmed unrestricted access across services

## Step 4: Identify Risk
- User had full control over AWS resources
- No restrictions on actions or services

## Step 5: Create Custom Restricted Policy
Created policy allowing only S3 read access:

## Step 6: Replace Policy
- Removed `AdministratorAccess`
- Attached custom policy

## Step 7: Re-Test Access
- Could view S3 buckets
- Could NOT:
  - Upload files
  - Delete files
  - Launch EC2

## Step 8: Compare Behavior
- Before: full unrestricted access
- After: limited to specific actions
