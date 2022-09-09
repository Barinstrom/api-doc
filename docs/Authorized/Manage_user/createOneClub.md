---
sidebar_position: 2
---

# /:schoolID/add-club

ใช้สำหรับการเพิ่มชมรมเพียง 1 ชมรม ในกรณีที่จะต้องทำการสร้างเพิ่มเติม

**Method** `POST`

**Role ที่ใช้ได้** `teacher` , `system admin`

**content-type** `application/json`

|PATH variable |Descripton|
|-----|--------|
|schoolID|เลข ID ของแต่ละโรงเรียน |

```json title="Request"
{
    "clubName": "name",
    "category": "science",
    "clubInfo": "lorem ipsum",
    "count": 0,
    "limit": 30,
    "teacherID": "12345",
    "year": 2565,
    "schedule": "15:00-16:00",
    "reviews":["reviews1",],
    "picture": {"pictureID":123, "urlPicture":"www.abc.com/picture/download"}

}
```

```json title="Response"
{
  "success": true,
}
```