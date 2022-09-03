---
sidebar_position: 2
---

# /auth/not_approved


ใช้สำหรับการดึงทุกโรงเรียนที่ไม่ผ่านการ approve 


**Method** `GET`

**Role ที่ใช้ได้** `system admin`

**content-type** `application/json`

```json title="Request"
{
    ส่งเลขเพจสำหรับ pagination
}
```

```json title="Response"
{
  array list โรงเรียนทุกโรงเรียน ที่ not_approve
}
```