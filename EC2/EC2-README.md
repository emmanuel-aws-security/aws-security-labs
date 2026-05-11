# EC2 Security & Debugging Lab

## 🎯 Lab Goal

This lab focused on deploying and troubleshooting AWS EC2 infrastructure while simulating common real-world failure conditions that affect cloud-hosted applications.

The objective was not only to launch an EC2 instance, but to understand how compute services fail, how connectivity problems are diagnosed, and how layered cloud troubleshooting works in practice.

---

## 🧪 Environment Setup

In this lab I configured and tested:

- EC2 instances running Linux
- nginx web server deployment
- SSH remote access using key pairs
- Security groups controlling inbound traffic
- Public IP connectivity testing
- Local and remote service validation

The environment was designed to simulate common operational and security issues found in cloud-hosted systems.

---

## 🔥 Failure Scenarios Simulated

I intentionally introduced multiple failure conditions to practice systematic troubleshooting, including:

- Stopping nginx services to simulate application downtime
- Blocking HTTP traffic through security group misconfiguration
- Testing inaccessible ports and connection failures
- Investigating local vs external connectivity differences
- Verifying service behavior using logs and command-line tools

These scenarios helped demonstrate how cloud issues often involve multiple interconnected layers rather than a single point of failure.

---

## 🔍 Debugging & Investigation Workflow

During troubleshooting, I followed a structured investigation process instead of guessing:

1. Verify whether the service is running
2. Test local access using curl localhost
3. Check listening ports and active connections
4. Review security group rules
5. Analyze system and application logs
6. Compare local functionality vs external accessibility

This process helped isolate whether failures originated from the application layer, operating system, network configuration, or AWS infrastructure settings.

---

## 🧠 Key Technical Learnings

This lab reinforced several important cloud operations and security concepts:

- EC2 issues are often caused by configuration errors rather than infrastructure failure
- Security groups directly affect application accessibility
- Successful SSH access does not guarantee application availability
- Local testing helps isolate network-related problems
- Effective debugging requires validating each infrastructure layer methodically

The lab also improved my ability to troubleshoot Linux-based cloud environments using logs, service status checks, and network validation tools.

---

## ⚠️ Real-World Security Insight

Many “server down” incidents are not caused by crashed infrastructure.

In cloud environments, outages frequently result from:
- incorrect security group rules
- blocked ports
- stopped services
- permission issues
- routing or networking mistakes

This lab focused on identifying those conditions systematically instead of relying on assumptions or trial-and-error troubleshooting.
