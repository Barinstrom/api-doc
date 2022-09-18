---
sidebar_position: 5
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/update-student


ใช้สำหรับการ update ข้อมูล student

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
    "enteredYear": "2022",
    "classYear": 1,
    "isActive": 1,
    "tel": "0123456789",
    "email": "email.s@ku.th",
    "clubs": "",
    "reviews": "",
    "requests": ""
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