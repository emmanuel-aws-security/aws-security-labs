# VPC Lab — NAT Gateway Learnings

## 🔴 Core Concept
NAT Gateway allows private instances to access the internet WITHOUT being exposed.

## 🧠 Key Insight
Traffic flow:

Private EC2 → NAT Gateway → Internet

BUT:

Internet → Private EC2 ❌ (blocked)

## 🔍 What Happened
- Before:
  No route → no internet

- After:
  Route → NAT → outbound access works

## ⚠️ Critical Understanding
NAT Gateway:
- does NOT allow inbound traffic
- only supports outbound connections

## 🧠 Real-World Use Case
- Application servers in private subnet
- Databases in private subnet
- Only web layer is public

## 🧾 Final Conclusion
Secure architectures separate:
- public access (via public subnet)
- internal services (via private subnet + NAT)
