---
sidebar_position: 2
---

# /auth/:schoolID/status


ใช้สำหรับตรวจสอบว่าโรงเรียนไอดีนี้ status เป็นอะไร

**Method** `POST`

**Role ที่ใช้ได้** `system admin`

**content-type** `application/json`

```json title="Request"
{
    ส่ง ไอดี ของโรงเรียน
}
```

```json title="Response"
{
  status ของโรงเรียนนั้นๆว่า approve, not_approved, pending
}
```