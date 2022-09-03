---
sidebar_position: 2
---

# /auth/:schoolID/edit


ใช้สำหรับแก้ไขข้อมูลของ school admin

**Method** `POST`

**Role ที่ใช้ได้** `system admin`

**content-type** `application/json`

```json title="Request"
{
    สามารถแก้ไขรายละเอียดของ school admin ได้    
}
```

```json title="Response"
{
  การแก้ไขนั้น สำเร็จ, ไม่สำเร็จ, error
}
```