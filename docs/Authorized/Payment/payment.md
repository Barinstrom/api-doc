---
sidebar_position: 1
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /payment


ใช้สำหรับตรวจสอบว่า `paymentIntentId` ของโรงเรียนนั้นได้มีการชำระเงินแล้วหรือยัง หากมีการชำระเงินแล้ว

ระบบจะทำการเปลี่ยนสถานะการชำระเงินของโรงเรียนให้เป็น `success`

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