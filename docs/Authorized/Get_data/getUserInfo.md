---
sidebar_position: 1
---

# /:schoolID/user


ใช้สำหรับการดูข้อมูลส่วนตัวของแต่ละ User

**Method** `GET`

**Role ที่ใช้ได้** `system admin`, `teacher`, `student`

**content-type** `application/json`

**PATH variable** 

|PATH variable |Descripton|
|-----|--------|
|schoolID|เลข ID ของแต่ละโรงเรียน       |


```json title="Response"
{
  "success": true,
  "data": {
    "email": "negomor671@xitudy.com",
    "school": "promma",
    "role": "admin",
    "status": "Pending",
    "confirmationCode": "vXJTtyZGDZMmputizRX2qr4ew",
    "_id": "6310c1835c4f87dc9e92875a",
    "__v": 0
  }
}
```