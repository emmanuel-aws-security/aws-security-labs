🧠 VPC TROUBLESHOOTING CHECKLIST 


🧪 VPC INCIDENT ROUTINE (SITE / CONNECTION NOT WORKING)
🔴 STEP 1 — Is the instance even reachable?
Is EC2 running?
Does it have:
public IP (if expected)
correct subnet?
👉 If NO → problem is deployment layer, not network

🔴 STEP 2 — Subnet check (public or private?)
Ask:
Is it in public subnet or private subnet?
Check:
Public subnet → should have route to IGW
Private subnet → no direct internet access
👉 If private subnet:
internet access failure is EXPECTED


🔴 STEP 3 — Route Table check (MOST COMMON ISSUE)
Check:

Does subnet route include:
0.0.0.0/0 → Internet Gateway
OR for private:
0.0.0.0/0 → NAT Gateway
👉 If missing → NO INTERNET ACCESS

🔴 STEP 4 — Security Group check
Ask:

Does SG allow required port?
Examples:
HTTP → port 80
SSH → port 22
Check:
inbound rules
source (0.0.0.0/0 or restricted IP)
👉 If blocked → connection fails even if network is correct

🔴 STEP 5 — NACL check (silent blocker)
Ask:
Is subnet NACL blocking traffic?
Check:
inbound rules
outbound rules
explicit DENY rules
👉 If DENY exists → traffic blocked EVEN if SG allows it

🔴 STEP 6 — Internal test (IS IT EVEN THE NETWORK?)
From EC2:
curl http://localhost
Interpret:
works → app is fine
fails → app issue (not network)

🔴 STEP 7 — External test
From your machine:
curl http://PUBLIC-IP
Interpret:
fails but localhost works → network issue
fails both → service issue

🔴 STEP 8 — Flow Logs (if enabled)
Check:
ACCEPT → traffic allowed
REJECT → blocked by SG or NACL






If you want next, I can turn this into:
👉 a GitHub “VPC Debug Playbook” markdown file you can literally reuse in interviews and labs
