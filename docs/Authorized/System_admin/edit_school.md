---
sidebar_position: 2
---

# /:schoolID/edit


ใช้สำหรับแก้ไขข้อมูลของ school admin 

**Method** `PATCH`

**Role ที่ใช้ได้** `system admin`

**content-type** `application/json`

```json title="Request"
{
      schoolName:"Jumpada",
      urlLogo:"mylogo",
      bgColor:"teal"
}
```

```json title="Response"
{
  "success": false,
  "message": "update fail"
}
```
