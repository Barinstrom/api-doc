---
sidebar_position: 2
---

# /:schoolID/student/ownclub


ใช้เรียกชุมนุมที่ตนเองลงทะเบียนสำเร็จ



**Method** `GET`

**Role ที่ใช้ได้** `student`

**content-type** `application/json`



**Response**

ส่งมาเป็น list ของ `body` ของ `club` ที่นักเรียนได้ลงทะเบียนสำเร็จ

```json title="Response (Parginate)"
{
  //ข้อมูล club
  "clubID": "ipsum",
  "category":"ipsum",
  "clubInfo":"ipsum",
  "review":"ipsum",
  "schedule":
  
}
```

