# IAM Mini Attack Scenario — Investigation

## 🧠 Problem Detected
User has full access to AWS resources. Need to confirm permission source.

---

## 🔍 Step 1: IAM Policy Simulator

Tested:
- Service: S3
- Action: GetObject

Result:
- ✅ Allowed or ❌ Denied (based on policy simulation)

Checked result details:
- Policy source: AdministratorAccess
- No explicit deny found

---

## 🔍 Step 2: Manual Permission Trace

Checked all layers:

### 1. User Policy
- AdministratorAccess attached

### 2. Group Policy
- None (or inherited admin access)

### 3. Permissions Boundary
- Not set

### 4. Resource Policy (S3)
- No restrictions applied

---

## ⚠️ Conclusion
User has unrestricted access due to AdministratorAccess policy.
