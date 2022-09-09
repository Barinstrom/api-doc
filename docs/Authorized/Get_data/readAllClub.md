---
sidebar_position: 2
---

# /:schoolID/clubs


ใช้สำหรับดูว่าโรงเรียนที่สังกัดมีชุมนุมใดบ้าง


**Method** `GET`

**Role ที่ใช้ได้** `teacher`, `system admin`, `student`

**content-type** `application/json`

|PATH variable |Descripton|
|-----|--------|
|schoolID|เลข ID ของแต่ละโรงเรียน |

```json title="Request (Parginate)"
{
  // ส่งเลขสำหรับ Pagination 
  // query
}
```


```json title="Response (Parginate)"
{
  "clubs":["club1","club2"]
  //เป็น list ของ club ในโรงเรียนนั้น ๆ 
}
```