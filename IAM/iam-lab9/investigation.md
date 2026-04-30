# Investigation — Why Was Data Exposed?

## 🧠 Problem
An S3 object was accessible publicly without authentication.

---

## 🔍 Step 1: IAM Policy Simulation

Tested action:
- s3:GetObject

Result:
- ❌ Denied (from IAM user perspective)

Observation:
- IAM policies did NOT grant access to the object

---

## 🔍 Step 2: Public Access Verification

- Accessed object via direct URL (no login)
- Object was successfully retrieved

Observation:
- Access was possible without IAM authentication

---

## 🔍 Step 3: S3 Bucket Policy Analysis

Checked bucket policy in:
👉 :contentReference[oaicite:0]{index=0}

Findings:
- Principal: "*"
- Action: s3:GetObject
- Effect: Allow

Interpretation:
- Policy allows ANY user (including anonymous/public users) to read objects

---

## 🔥 Root Cause
Access was granted by the S3 bucket policy, not IAM identity-based policies.

---

## ⚠️ Key Insight

AWS evaluates access using multiple policy layers:
- IAM policies (identity-based)
- Resource policies (e.g. S3 bucket policies)

Even if IAM denies access:
- A resource policy can still grant public access

---

## 🧾 Conclusion
The data exposure occurred due to a permissive bucket policy allowing public read access (`Principal: "*"`) rather than an IAM misconfiguration.# Investigation — Why Was Data Exposed?

## 🧠 Problem
An S3 object was accessible publicly without authentication.

---

## 🔍 Step 1: IAM Policy Simulation

Tested action:
- s3:GetObject

Result:
- ❌ Denied (from IAM user perspective)

Observation:
- IAM policies did NOT grant access to the object

---

## 🔍 Step 2: Public Access Verification

- Accessed object via direct URL (no login)
- Object was successfully retrieved

Observation:
- Access was possible without IAM authentication

---

## 🔍 Step 3: S3 Bucket Policy Analysis

Checked bucket policy in:
👉 :contentReference[oaicite:0]{index=0}

Findings:
- Principal: "*"
- Action: s3:GetObject
- Effect: Allow

Interpretation:
- Policy allows ANY user (including anonymous/public users) to read objects

---

## 🔥 Root Cause
Access was granted by the S3 bucket policy, not IAM identity-based policies.

---

## ⚠️ Key Insight

AWS evaluates access using multiple policy layers:
- IAM policies (identity-based)
- Resource policies (e.g. S3 bucket policies)

Even if IAM denies access:
- A resource policy can still grant public access

---

## 🧾 Conclusion
The data exposure occurred due to a permissive bucket policy allowing public read access (`Principal: "*"`) rather than an IAM misconfiguration.
