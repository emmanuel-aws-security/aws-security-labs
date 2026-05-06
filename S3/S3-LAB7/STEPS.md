# Steps — Setup & Exposure

----------------------------------
## 🔹 Phase 1: Weak Setup
----------------------------------

- Create S3 bucket
- Upload sensitive file (e.g. credentials.txt)
- Disable block public access
- Apply public read (object or bucket policy)

----------------------------------
## 🔹 Phase 2: Confirm Exposure
----------------------------------

- Copy object URL
- Open in browser

Result:
- File accessible without login ✅
