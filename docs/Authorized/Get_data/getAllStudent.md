---
sidebar_position: 2
---

# /auth/:schoolID/getallstudent


ใช้เรียกข้อมูล student ทั้งหมด



**Method** `GET`

**Role ที่ใช้ได้** `school admin, system admin`

**content-type** `application/json`



**Response** ส่งมาเป็น `list` ของ `body` ของ `student` 

```json title="Response (Parginate)"
{
  "student":[{"student1"},{"student2"}]
  //เป็น list ของ student ในโรงเรียนนั้น ๆ 
}
```

