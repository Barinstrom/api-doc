---
sidebar_position: 3
---

# /:schoolID/student/pastclubs


ใช้เรียกชุมนุมที่ตนเองผ่านการเรียนมาแล้ว (ได้รับเกรด ผ่าน มาแล้ว)



**Method** `GET`

**Role ที่ใช้ได้** `student`

**content-type** `application/json`

|PATH variable |Descripton|
|-----|--------|
|schoolID|เลข ID ของแต่ละโรงเรียน |

**Response**

ส่งมาเป็น list ของ `body ของ club` ที่ตนเองผ่านการเรียนมาแล้ว

```json title="Response (Parginate)"
{
  "clubs":[{"club1"},{"club2"}]
}
```


