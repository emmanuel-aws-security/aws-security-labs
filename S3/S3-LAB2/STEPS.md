# S3 Lab — Public vs Private Steps

----------------------------------
## 🔹 Step 1: Create Bucket (Private)
----------------------------------

- Create S3 bucket (default settings)
- Upload a test file (e.g. test.txt)

----------------------------------
## 🔹 Step 2: Attempt Public Access (Should Fail)
----------------------------------

- Copy object URL
- Open in browser

Result:
- Access Denied ❌

----------------------------------
## 🔹 Step 3: Make Object Public
----------------------------------

- Go to object permissions
- Disable block public access (if required)
- Grant public read access

----------------------------------
## 🔹 Step 4: Access Again
----------------------------------

- Open same URL in browser

Result:
- File loads successfully ✅

----------------------------------
## 🔹 Step 5: Revert (IMPORTANT)
----------------------------------

- Remove public access
- Confirm access denied again
