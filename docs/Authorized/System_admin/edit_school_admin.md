---
sidebar_position: 2
---

# /:schoolID/edit_admin


ใช้สำหรับแก้ไขข้อมูลของ school admin 

**Method** `PATCH`

**Role ที่ใช้ได้** `system admin`

**content-type** `application/json`

```json title="Request"
{
    "email" : "user@gmail.com",
    "password" : "password",
    "tel" : "0959608937"
}
```

```json title="Response"
{
  message "error or succes"
}
```
