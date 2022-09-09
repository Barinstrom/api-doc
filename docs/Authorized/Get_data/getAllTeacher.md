---
sidebar_position: 2
---

# /:schoolID/teachers


ใช้เรียกข้อมูล teacher ทั้งหมด โดยsearchตามschoolID



**Method** `GET`

**Role ที่ใช้ได้** `school admin, system admin`

**content-type** `application/json`



**Response**

ส่งมาเป็น `list` ของ `body` ของ `teacher` 

```json title="Response (Parginate)"
{
  "teacher":[{"teacher1"},{"teacher2"}]
  //เป็น list ของ teacher ในโรงเรียนนั้น ๆ 
}
```

