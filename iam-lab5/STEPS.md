# IAM Lab 5 — Steps

## Step 1: Create IAM User
- Used existing IAM user 

## Step 2: Create Access Key
- Generated access key and secret key for the user
- Downloaded or copied credentials

## Step 3: Configure AWS CLI
- Ran:
  aws configure
- Entered:
  - Access Key
  - Secret Key
  - Region

## Step 4: Test Access
- Ran:
  aws s3 ls
- Confirmed access to S3 resources
  Verify CLI Identity
- Ran `aws sts get-caller-identity`
- Confirmed IAM user identity (dev-user)
  
## Step 6: Test S3 Access via CLI
- Ran `aws s3 ls` → successful (read access confirmed)
- Attempted upload via CLI → Access Denied
- Confirmed read-only policy enforcement
- 
## Step 7: Simulate Risk
- Noted that anyone with the access key can run the same commands from anywhere

## Step 8: Cleanup (IMPORTANT)
- Deleted or deactivated the access key
