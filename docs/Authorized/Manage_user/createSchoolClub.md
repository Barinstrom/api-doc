---
sidebar_position: 2
---

# /:schoolID/add-clubs

ใช้สำหรับการสร้างชุมนุมขึ้นมาใหม่ จะทำการสร้างชุมนุมที่อยู่ภายในโรงเรียนนั้น ๆ มาให้โดยอัตโนมัติจากไฟล์ CSV ที่ทางโรงเรียนให้มา

**Method** `POST`

**Role ที่ใช้ได้** `school admin` , `system admin`

**content-type** `application/json`

|PATH variable |Descripton|
|-----|--------|
|schoolID|เลข ID ของแต่ละโรงเรียน |

```json title="Request"
{
    "downloadlink":"www.def.com/download"
}
```

```json title="Response"
{
  "success": true,
}
```