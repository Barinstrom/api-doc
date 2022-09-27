---
sidebar_position: 6
---

# /:schoolID/add-clubs

ใช้สำหรับการสร้างชุมนุมขึ้นมาใหม่ จะทำการสร้างชุมนุมที่อยู่ภายในโรงเรียนนั้น ๆ มาให้โดยอัตโนมัติจากไฟล์ CSV ที่ทางโรงเรียนให้มา

**Method** `POST`

**Role ที่ใช้ได้** `school admin` , `system admin`

**content-type** `application/json`

```json title="Request"
{
    {
    "teacherID": "631c7471c729fbbe1a959b32",
    "clubName": "club1",
    "groupID": "1",
    "category": "science",
    "clubInfo": "lorem ipsum",
    "limit": 30,
    "schoolYear": 2565,
    "schedule": ["15:00-16:00"],
    "picture": {"pictureID":123, "urlPicture":"www.abc.com/picture/download"}
    },
    {
    "teacherID": "631c7471c729fbbe1a959b32",
    "clubName": "club2",
    "groupID": "2",
    "category": "science",
    "clubInfo": "lorem ipsum",
    "limit": 30,
    "schoolYear": 2565,
    "schedule": ["15:00-16:00"],
    "picture": {"pictureID":123, "urlPicture":"www.abc.com/picture/download"}
    },

}
```

```json title="Response"
{
  "success": true,
}
```