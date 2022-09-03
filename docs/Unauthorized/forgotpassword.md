---
sidebar_position: 4
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /forgotpassword


ใช้สำหรับการ reset password สำหรับผู้ใช้ที่ลืมรหัสผ่าน เมื่อเรียก request ดังกล่าว ระบบจะส่ง Link Reset password ไปยัง email ของผู้ใช้

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
  "message": "Email has been sent,Please check your email.",
}
```
</TabItem>

<TabItem value="fail">

```json title="Response"
{
  "message": "Email is not exist on database..",
}
```
</TabItem>

</Tabs>