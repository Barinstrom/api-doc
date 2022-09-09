---
sidebar_position: 2
---

# /schools/pending


ใช้สำหรับการดึงทุกโรงเรียนที่อยู่ในสถานนะ pending โดยสามารถที่จะ search ได้ด้วย

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
  array list โรงเรียนทุกโรงเรียน ที่ pending
}
```