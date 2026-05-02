# EC2 Debug Lab — Case 3 Steps

----------------------------------
## 🔹 BASELINE — Confirm Working
----------------------------------

- curl http://localhost → works
- curl http://PRIVATE-IP → works
- browser (public IP) → works

----------------------------------
## 🔹 SCENARIO 1 — Network Issue
----------------------------------

### Break It
- Remove port 80 from Security Group

### Test
- curl localhost → fails
- curl PRIVATE-IP → works ✅
- browser → fails ❌

### Conclusion
- Service is fine
- Network is blocking external access

### Fix
- Re-add port 80 to Security Group

----------------------------------
## 🔹 SCENARIO 2 — Service Failure
----------------------------------

### Break It
- Stop nginx:
  sudo systemctl stop nginx

### Test
- curl localhost → fails ❌
- curl PRIVATE-IP → fails ❌
- browser → fails ❌

### Conclusion
- Application/service is down

### Fix
- Start nginx:
  sudo systemctl start nginx






