---
sidebar_position: 2
---

# /auth/pending


ใช้สำหรับการดึงทุกโรงเรียนที่อยู่ในสถานนะ pending 

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
  array list โรงเรียนทุกโรงเรียน ที่ pending
}
```