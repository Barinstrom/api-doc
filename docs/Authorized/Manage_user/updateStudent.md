---
sidebar_position: 2
---

# /auth/:schoolID/updatestudent


ใช้สำหรับการ update ข้อมูล student

**Method** `PUT`

**Role ที่ใช้ได้** `school admin` , `system admin`

**content-type** `application/json`

```json title="Request"
{
    "firstname": "first",
    "lastname": "last",
    "enteredYear": "2022",
    "classYear": 1,
    "isActive": 1,
    "tel": "0123456789",
    "email": "email.s@ku.th",
    "clubs": "",
    "reviews": "",
    "requests": ""
}
```

```json title="Response"
{
  "success": true
}
```