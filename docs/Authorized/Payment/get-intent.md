---
sidebar_position: 1
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /get-intent


ใช้สำหรับสร้าง `paymentIntentId` เพื่อใช้ระบุตัวตนในการชำระเงินต่อไป

โดยจะใช้ endpoint นี้ได้ก็ต่อเมื่อสถานะการชำระเงินของโรงเรียนเป็น `pending` อยู่เท่านั้น

**Method** `GET`

**Role ที่ใช้ได้** `school admin`


<Tabs
  groupId="type"
  defaultValue="success"
  values={[
    { label: 'Success', value: 'success', },
    { label: 'fail', value: 'fail', },
  ]
}>

<TabItem value="success">

```json title="Response"
{
  "success": true,
}
```
</TabItem>

<TabItem value="fail">

```json title="Response"
{
  "success": false,
  "messege": "Lorem Ipsum"
}
```
</TabItem>


</Tabs>