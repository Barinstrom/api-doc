---
sidebar_position: 2
---

# /auth/:schoolID/updateteacher


ใช้สำหรับการ update ข้อมูล teacher

**Method** `PUT`

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