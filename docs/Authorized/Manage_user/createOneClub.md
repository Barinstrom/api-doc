---
sidebar_position: 5
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/add-club

ใช้สำหรับการเพิ่มชุมนุมเพียง 1 ชุมนุม 

**Method** `POST`

**Role ที่ใช้ได้** `school admin` , `system admin`

**content-type** `application/json`

```json title="Request"
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
  "message": "Club name is already exists."
}
```
</TabItem>

</Tabs>
