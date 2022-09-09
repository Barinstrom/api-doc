---
sidebar_position: 3
---

# /:schoolID/teacher/pastclubs


ใช้เรียกชุมนุมที่ตนเองผ่านการเรียนมาแล้ว (ได้รับเกรด ผ่าน มาแล้ว)



**Method** `GET`

**Role ที่ใช้ได้** `teacher`

**content-type** `application/json`



**Response**

ส่งมาเป็น list ของ `body ของ club` ที่ตนเองผ่านการเรียนมาแล้ว

```json title="Response (Parginate)"
{
  "clubs":[{"club1"},{"club2"}]
  //เป็น list ของ club ในโรงเรียนนั้น ๆ 
}
```


