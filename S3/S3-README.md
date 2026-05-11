# S3 Security Lab

## 🎯 Lab Goal

This lab focused on understanding how data storage security works in AWS using S3 buckets, and how incorrect permissions can expose sensitive information publicly.

The objective was to learn how S3 access is controlled, how storage exposure happens, and why proper bucket configuration is critical in cloud environments.

---

## 🧪 Environment Setup

In this lab I configured and tested:

- S3 buckets with different access settings
- Public and private storage configurations
- File uploads and object retrieval
- Bucket policies and permission rules
- Controlled access scenarios between users and resources

The environment was designed to compare secure storage practices against intentionally exposed configurations.

---

## 🔥 Security Scenarios Tested

I intentionally tested several storage security situations, including:

- Public vs private object accessibility
- Bucket policy misconfigurations
- Exposure risks caused by incorrect permissions
- Access behavior for different bucket settings
- File retrieval from public and restricted buckets

These scenarios helped demonstrate how small permission mistakes can expose large amounts of data unintentionally.

---

## 🔍 Access Validation & Testing

During testing, I verified:

1. Whether bucket contents were publicly accessible
2. How bucket policies affected object visibility
3. Differences between private and public access behavior
4. How permission changes immediately affected exposure
5. Which configurations created unnecessary risk

This helped build a clearer understanding of how S3 permissions directly affect cloud data security.

---

## 🧠 Key Technical Learnings

This lab reinforced several important cloud storage security concepts:

- S3 security depends heavily on correct permission configuration
- Public access settings can override expected restrictions
- Storage exposure can happen even when infrastructure itself is secure
- Bucket policies must be reviewed carefully to avoid accidental exposure
- Data protection in cloud environments starts with proper access control

The lab also improved my understanding of how AWS storage services manage accessibility and security at scale.

---

## ⚠️ Real-World Security Insight

S3 misconfiguration is one of the most common causes of cloud data exposure.

A single overly permissive bucket policy can unintentionally expose:
- sensitive company files
- backups
- internal documents
- application data

This lab focused on understanding how those exposures happen and how proper configuration reduces storage-related security risk in AWS environments.
