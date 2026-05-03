# EC2 Breach Simulation — Steps

----------------------------------
## 🔹 PHASE 1 — Weak Setup (Intentional Misconfiguration)
----------------------------------

### Step 1: Launch EC2
- Public instance created
- SSH enabled from 0.0.0.0/0

### Step 2: Install Web Server
sudo apt install nginx -y

### Step 3: Store Fake Credentials (Risk Simulation)
echo "AWS_ACCESS_KEY=FAKE123" > creds.txt

----------------------------------
## 🔹 PHASE 2 — Attack Thinking
----------------------------------

### Threat Model Questions:
- If attacker accesses this instance, what can they see?
- Can they read files?
- Can they find credentials?
- Can they access AWS services?

### Potential Impact:
- Credential theft
- S3 data access
- Infrastructure takeover
