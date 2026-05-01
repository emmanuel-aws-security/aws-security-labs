# EC2 Lab 4 — Learnings

## 🔴 Core Concept
Public instances are accessible from the internet, while private instances are isolated inside a VPC.

## 💥 Real-World Impact
Databases and internal services must never be exposed publicly. Doing so creates serious data breach risk.

## ⚠️ Why Private Subnets Matter
- They prevent direct internet access
- They reduce attack surface
- They enforce controlled communication paths

## 🧠 Security Insight
Access to private instances should only happen through:
- Bastion hosts
- VPNs
- Internal network routing

  Instance has no public IP and cannot be reached from the internet, confirming network-level isolation


  “Although the instance is not publicly reachable, it is not inherently secure. If another internal resource is compromised, this instance could still be accessed.”
  
## 🧾 Final Conclusion
Network design is as important as firewall rules. Public exposure should be intentional, not accidental.
