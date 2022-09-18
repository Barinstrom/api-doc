---
sidebar_position: 6
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/update-teacher


ใช้สำหรับการ update ข้อมูล teacher

**Method** `PATCH`

**Role ที่ใช้ได้** `school admin` , `system admin`

**content-type** `application/json`

|PATH variable |Descripton|
|-----|--------|
|schoolID|เลข ID ของแต่ละโรงเรียน |

```json title="Request"
{
    "firstname": "first",
    "lastname": "last",
    "tel": "0123456789",
    "email": "email.s@ku.th",
    "clubs": ""
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