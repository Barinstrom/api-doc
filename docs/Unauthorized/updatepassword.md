---
sidebar_position: 5
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /updatepassword


ใช้สำหรับการ update password เมื่อผู้ใช้กด Reset password link แล้วกรอกรหัสผ่านที่ต้องการเปลี่ยนเรียบร้อยแล้ว

**Method** `POST`

**content-type** `application/json`

```json title="Request"
{
    "email": "negomor671@xitudy.com",
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
  "message": "Your password has been changed.",
}
```
</TabItem>

<TabItem value="fail">

```json title="Response"
{
  "message": "Incorrect token or it is expired.",
}
```
</TabItem>

</Tabs>