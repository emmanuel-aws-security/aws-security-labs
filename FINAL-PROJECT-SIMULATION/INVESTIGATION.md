# Investigation Process

## 🎯 Goal
Identify:
- what happened
- who performed actions
- where exposure existed

---

## 🔍 Investigation Areas

### EC2 Investigation
Checked:
- service status
- open ports
- local connectivity
- logs

Commands used:

systemctl status nginx
ss -tulnp
curl localhost
journalctl -u nginx

---

### CloudTrail Investigation
Reviewed:
- IAM activity
- S3-related actions
- source IP addresses
- timestamps

Questions answered:
- Who performed the action?
- When did it happen?
- From where?

---

### CloudWatch Investigation
Observed:
- CPU activity
- instance health
- alarm states

Purpose:
- detect unhealthy behavior
- confirm monitoring visibility

---

## 🧠 Findings
Identified:
- overexposed SSH access
- public S3 exposure
- excessive IAM permissions
- weak network isolation
