# Fix — Resolving Policy Conflicts

## 🔧 Step 1: Identify Redundant Policies
- Found overlapping S3 permissions across user and group

## 🔧 Step 2: Remove Conflicts
- Removed direct user full-access policy

## 🔧 Step 3: Keep Clean Structure
- Group policy = read-only access
- Explicit deny = only for critical delete protection

## 🔧 Step 4: Re-Test
- s3:ListBucket → Allowed
- s3:PutObject → Denied
- s3:DeleteObject → Denied

---

## 🧠 Final Result
Access is now predictable and controlled.
