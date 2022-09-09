---
sidebar_position: 2
---

# /schools/approved


ใช้สำหรับการดึงทุกโรงเรียนที่ผ่านการ approve โดยสามารถที่จะ search ได้ด้วย

**Method** `GET`

**Role ที่ใช้ได้** `system admin`

**content-type** `application/json`

```json title="Request"
{
    "page" : number,
    "query" : {
      "schoolName": string,
    },
}
```

```json title="Response"
{
  ชื่อรร email
  
  [array list โรงเรียนทุกโรงเรียน ที่ approve]
}
```