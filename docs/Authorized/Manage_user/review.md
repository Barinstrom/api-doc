---
sidebar_position: 7
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/add-review


ใช้เพิ่ม review ชุมนุมที่ตนเองได้ผ่านการเรียนมาแล้ว โดยระบบจะทำการตรวจสอบเองว่า นักเรียนคนดังกล่าวผ่านการเรียนวิชาที่กำลังจะ review แล้วหรือไม่

**Method** `POST`

**Role ที่ใช้ได้** `student`

**content-type** `application/json`

```json title="Request"
{
    "clubID" : "631c6e5cb0f33e324f1b1e3c",
    "studentID" : "631ed901cbc23688f173c15f",
    "textReview" : "วิชานี้ดีมากเลยครับ"
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
  "message": "You are not allow to comment this subject."
}
```
</TabItem>

</Tabs>


