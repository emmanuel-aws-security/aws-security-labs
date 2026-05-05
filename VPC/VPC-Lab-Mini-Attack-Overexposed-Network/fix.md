# Fix — Securing Overexposed Network

## 🔧 Fix 1 — Restrict SSH
- Change Security Group:
  FROM: 0.0.0.0/0
  TO: your IP /32

## 🔧 Fix 2 — Use Private Subnet for Sensitive Systems
- Move backend / sensitive workloads to private subnet

## 🔧 Fix 3 — Add Proper Segmentation
- Public subnet → only web layer
- Private subnet → internal systems only

## 🔧 Fix 4 — Reduce Attack Surface
- Close unused ports
- Remove unnecessary public exposure

## 🧠 Final State
- SSH access restricted
- Sensitive systems isolated
- No open world access by default
