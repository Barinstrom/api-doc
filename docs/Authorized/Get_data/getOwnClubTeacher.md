---
sidebar_position: 2
---

# /:schoolID/teacher/ownclubs


ใช้เรียกชุมนุมที่ตนเองลงทะเบียนสำเร็จ



**Method** `GET`

**Role ที่ใช้ได้** `teacher`

**content-type** `application/json`



**Response**

ส่งมาเป็น list ของ `body` ของ `club` ที่นักเรียนได้ลงทะเบียนสำเร็จ

```json title="Response (Parginate)"
{
  "clubs":[{"club1"},{"club2"}]
}
```

