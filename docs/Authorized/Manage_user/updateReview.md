---
sidebar_position: 10
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/update-review


ใช้แก้ไข review ของตนเอง

**Method** `PATCH`

**Role ที่ใช้ได้** `student`

**content-type** `application/json`

|PATH variable |Descripton|
|-----|--------|
|schoolID|เลข ID ของแต่ละโรงเรียน |


```json title="Request"
{
    "reviewID" : "631c7c2cb025fb720c3eafb9",
    "textReview" : "วิชานี้ดีมาก ๆ เลยครับ"
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
  "message": "You are not allow to edit this review."
}
```
</TabItem>

</Tabs>


