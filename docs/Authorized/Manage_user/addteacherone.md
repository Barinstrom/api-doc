---
sidebar_position: 3
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/add-teacher


ใช้สำหรับการสร้าง user ที่มี role เป็น teacher ใน school ที่ระบุใน path parameter/variable :/schoolID หนึ่งคน และทำการส่ง activate token ไปทาง email ที่ได้ระบุไว้ โดยคนที่มีสิทธิ์การใช้จะมีเพียง user ที่มี role เป็น school admin ของโรงเรียนนั้น และ system admin เท่านั้น

**Method** `POST`


**Role ที่ใช้ได้** `school admin` , `system admin`


**content-type** `application/่json`


```json title="Request"
{
    "email": "negomor671@xitudy.com",
    "firstname": "aaaa",
    "lastname": "bbb",
    "tel": "0800000000",
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
  "success": true,
}
```
</TabItem>

<TabItem value="fail">

```json title="Response"
{
  "success": false,
  "message": "lorem ipsum",
}
```
</TabItem>

</Tabs>
