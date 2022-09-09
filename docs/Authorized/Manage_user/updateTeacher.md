---
sidebar_position: 6
---

# /:schoolID/update-teacher


ใช้สำหรับการ update ข้อมูล teacher

**Method** `PATCH`

**Role ที่ใช้ได้** `school admin` , `system admin`

**content-type** `application/json`

```json title="Request"
{
    "firstname": "first",
    "lastname": "last",
    "tel": "0123456789",
    "email": "email.s@ku.th",
    "clubs": ""
}
```

```json title="Response"
{
  "success": true
}
```