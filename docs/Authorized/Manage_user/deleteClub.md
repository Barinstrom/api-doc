---
sidebar_position: 11
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/delete-clubs


ใช้สำหรับการลบข้อมูล club ที่เราต้องการจะลบใน school ที่ระบุใน parameter :/school ตั้งแต่ 1 club ขึ้นไป โดยคนที่มีสิทธิ์การใช้จะมีเพียง user ที่มี role เป็น school admin ของโรงเรียนที่ club นั้นอยู่และ system admin เท่านั้น

**Method** `DELETE`


**Role ที่ใช้ได้** `school admin, system admin`


**content-type** `application/json`

|PATH variable |Descripton|
|-----|--------|
|schoolID|เลข ID ของแต่ละโรงเรียน |

```json title="Request"
{
    "clubs":[{"club1"},{"club2"}]
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