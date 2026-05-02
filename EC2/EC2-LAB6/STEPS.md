# EC2 Debug Lab — Case 1 Steps

## Step 1: Confirm Working State
- Verified nginx was running
- Tested:
  curl http://localhost
- Confirmed response

## Step 2: Break the Server (Simulate Failure)
- Stopped nginx:
  sudo systemctl stop nginx

## Step 3: Verify Failure
- Ran:
  curl http://localhost
- Observed failure (no response)

## Step 4: Investigate Service Status
- Checked:
  systemctl status nginx
- Observed service is inactive (dead)

## Step 5: Fix the Issue
- Restarted service:
  sudo systemctl start nginx

## Step 6: Verify Recovery
- Ran:
  curl http://localhost
- Confirmed response restored

## Step 7: Enable Persistence
- Ensured service starts on boot:
  sudo systemctl enable nginx
