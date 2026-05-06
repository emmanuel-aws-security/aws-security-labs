# S3 Exposure Attack — Steps

----------------------------------
## 🔹 Step 1: Create Bucket
----------------------------------

- Create S3 bucket
- Upload sensitive test file (e.g. secret.txt)

----------------------------------
## 🔹 Step 2: Enable Public Access
----------------------------------

- Disable block public access (if needed)
- Apply public read permissions

----------------------------------
## 🔹 Step 3: Confirm Exposure
----------------------------------

- Copy object URL
- Open in browser

Result:
- File accessible without login ✅
