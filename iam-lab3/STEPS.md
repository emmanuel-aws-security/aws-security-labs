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
