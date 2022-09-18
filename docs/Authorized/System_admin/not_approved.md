---
sidebar_position: 2
---

# /schools/not-approved?page=&query=


ใช้สำหรับการดึงทุกโรงเรียนที่ไม่ผ่านการ approve โดยสามารถที่จะ search ได้ด้วย


**Method** `GET`

**Role ที่ใช้ได้** `system admin`

```json title="query parameter"
{
    "page" : number,
    "query" : string,
}
```

```json title="Response"
{
  {
    "docs": [
        {
            "_id": "631c492bbcc0a793a998423e",
            "schoolID": "promma",
            "schoolName": "Prommanusorn Phetchaburi",
            "urlCertificateDocument": "https://res.cloudinary.com/tawanchai/image/upload/v1662792742/certificate_doc/rowir91414%40iunicus.com.png",
            "paymentStatus": "pending",
            "status": "not_approve",
            "paymentDate": "2022-09-10T08:22:03.658Z",
            "requests": [],
            "clubs": [],
            "adminID": [],
            "__v": 0,
            "schedule": []
        },
        {
            "_id": "6321d377740f04c2555e111c",
            "schoolID": "qwerty",
            "schoolName": "qwerty",
            "urlCertificateDocument": "https://res.cloudinary.com/tawanchai/image/upload/v1663161206/certificate_doc/tawanchai.ch%40ku.th.png",
            "paymentStatus": "pending",
            "status": "not_approve",
            "paymentDate": "2022-09-14T13:13:27.578Z",
            "requests": [],
            "clubs": [],
            "schedule": [],
            "adminID": [],
            "__v": 0
        }
    ],
    "totalDocs": 7,
    "limit": 2,
    "totalPages": 4,
    "page": 1,
    "pagingCounter": 1,
    "hasPrevPage": false,
    "hasNextPage": true,
    "prevPage": null,
    "nextPage": 2
}
}
```