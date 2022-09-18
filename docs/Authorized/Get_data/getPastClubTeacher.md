---
sidebar_position: 3
---

# /:schoolID/teacher/pastclubs


ใช้ดูชุมนุมที่ผ่านมาที่ตัวครูเคยเป็นที่ปรึกษา



**Method** `GET`

**Role ที่ใช้ได้** `teacher`

**content-type** `application/json`

|PATH variable |Descripton|
|-----|--------|
|schoolID|เลข ID ของแต่ละโรงเรียน |

**Response**

ส่งมาเป็น list ของ `body` ของ `club` ที่ครูเคยเป็นที่ปรึกษา

```json title="Response (Parginate)"
{
  "clubs":[{"club1"},{"club2"}]
}
```


