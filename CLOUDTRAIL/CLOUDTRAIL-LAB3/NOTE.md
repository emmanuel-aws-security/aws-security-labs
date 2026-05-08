## 🧠 Key Lesson Learned

CloudTrail visibility depends on:
- correct event type (management vs data events)
- correct configuration scope
- correct log destination (S3 / Lake)

Event History alone is NOT sufficient for S3 object-level investigation.

## ⚠️ Final Conclusion

This experiment shows that:
- CloudTrail Event History is limited
- S3 object-level tracking requires correct Data Event setup AND correct log source inspection

The absence of logs does NOT mean no activity occurred.
It means visibility was not correctly configured or checked in the right place.

