---
sidebar_position: 9
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/update-club


ใช้สำหรับการเปลี่ยนแปลงค่าในชมรม ในที่นี้คือสามารถระบุเจาะจงได้ว่าจะ update ค่าข้อมูลชมรมใด update ค่าใดบ้าง

**Method** `PATCH`

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

<Tabs
  groupId="type"
  defaultValue="success"
  values={[
    { label: 'success', value: 'success', },
    { label: 'fail', value: 'fail', }
  ]
}>

<TabItem value="success">

```json title="Response"
{
  "success": true
}
```
</TabItem>

<TabItem value="fail">

```json title="Response"
{
  "success": false,
  "message": "lorem ipsum."
}
```
</TabItem>

</Tabs>