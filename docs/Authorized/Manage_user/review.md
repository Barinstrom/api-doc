---
sidebar_position: 12
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/review


ใช้เพิ่ม review ชุมนุมที่ตนเองได้ผ่านการเรียนมาแล้ว โดยระบบจะทำการตรวจสอบเองว่านักเรียนคนดังกล่าวสามาถ review วิชาที่กำลังจะ review ได้หรือไม่

**Method** `POST`

**Role ที่ใช้ได้** `student`

**content-type** `application/json`

```json title="Request"
{
    "clubID": string_of_clubID,
    "message": "วิชานี้ดีมากเลยครับ",
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
  "message": "Comment success.",
}
```
</TabItem>

<TabItem value="fail">

```json title="Response"
{
  "message": "You are not allow to comment this subject.",
}
```
</TabItem>

</Tabs>


