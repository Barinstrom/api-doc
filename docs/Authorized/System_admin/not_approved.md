---
sidebar_position: 2
---

# /schools/not-approved


ใช้สำหรับการดึงทุกโรงเรียนที่ไม่ผ่านการ approve โดยสามารถที่จะ search ได้ด้วย


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
  array list โรงเรียนทุกโรงเรียน ที่ not_approve
}
```