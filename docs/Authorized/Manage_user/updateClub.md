---
sidebar_position: 2
---

# /auth/:schoolID/updateclub


ใช้สำหรับการเปลี่ยนแปลงค่าในชมรม ในที่นี้คือสามารถระบุเจาะจงได้ว่าจะ update ค่าข้อมูลชมรมใด update ค่าใดบ้าง

**Method** `PUT`

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
    "reviews":"",
    "picture": {"pictureID":123, "urlPicture":"www.abc.com/picture/download"}
    //ส่งมาแค่ field ที่ต้องทำการแก้ไขข้อมูล ไม่จำเป็นต้องส่งมาทั้งหมด
}
```

```json title="Response"
{
  "success": true,
}
```