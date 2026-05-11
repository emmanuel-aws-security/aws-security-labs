# VPC Networking Lab

## 🎯 Lab Goal

This lab focused on understanding how networking and isolation work inside AWS using Virtual Private Clouds (VPCs).

The objective was to learn how cloud environments control traffic flow, separate resources, and restrict exposure using network-level configurations instead of relying only on the server itself.

---

## 🧪 Environment Setup

In this lab I configured and tested:

- A custom VPC environment
- Public and private subnets
- Internet Gateway connectivity
- Route tables controlling traffic flow
- NAT Gateway for outbound internet access
- Security Groups and Network ACLs

The environment was structured to compare public-facing infrastructure against isolated internal infrastructure.

---

## 🔥 Networking Scenarios Tested

I intentionally tested several networking and access-control situations, including:

- Public subnet vs private subnet accessibility
- Route table misconfigurations
- Internet access behavior from different subnets
- Outbound-only connectivity using NAT Gateway
- Differences between Security Groups and Network ACLs
- Traffic restrictions between network layers

These tests helped demonstrate how network architecture directly affects system exposure and communication inside AWS environments.

---

## 🔍 Network Troubleshooting Approach

During testing, I practiced identifying where connectivity problems originated by checking:

1. Subnet placement
2. Route table configuration
3. Internet Gateway attachment
4. NAT Gateway routing
5. Security Group rules
6. Network ACL behavior

This helped build a clearer understanding of how multiple AWS networking components work together to allow or block traffic.

---

## 🧠 Key Technical Learnings

This lab reinforced several important cloud networking concepts:

- Network design strongly affects infrastructure security
- Public and private subnets behave differently by design
- Route tables determine where traffic is allowed to go
- NAT Gateways allow outbound internet access without exposing internal systems
- Security Groups and Network ACLs control traffic at different layers

The lab also improved my understanding of how AWS networking decisions impact accessibility, isolation, and overall environment structure.

---

## ⚠️ Real-World Security Insight

In AWS environments, isolation is enforced primarily through network architecture.

Even if a server is running correctly, poor network configuration can:
- expose internal systems publicly
- block legitimate traffic
- create unnecessary attack surface
- prevent systems from communicating properly

This lab focused on understanding how secure network segmentation reduces exposure and improves control over cloud environments.
