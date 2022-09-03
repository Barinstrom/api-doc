---
sidebar_position: 2
---

# /auth/approved


ใช้สำหรับการดึงทุกโรงเรียนที่ผ่านการ approve 

**Method** `POST`

**Role ที่ใช้ได้** `system admin`

**content-type** `application/json`

```json title="Request"
{
    ส่งเลขเพจสำหรับ pagination
}
```

```json title="Response"
{
  array list โรงเรียนทุกโรงเรียน ที่ approve
}
```