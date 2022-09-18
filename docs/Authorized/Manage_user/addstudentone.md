---
sidebar_position: 1
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/add-student


ใช้สำหรับการสร้าง user ที่มี role เป็น student ใน school ที่ระบุใน path parameter/variable :/school หนึ่งคน และทำการส่ง activate token ไปทาง email ที่ได้ระบุไว้ โดยคนที่มีสิทธิ์การใช้จะมีเพียง user ที่มี role เป็น school admin ของโรงเรียนนั้น และ system admin เท่านั้น

**Method** `POST`


**Role ที่ใช้ได้** `school admin` , `system admin`


**content-type** `application/่json`


```json title="Request"
{
    "email": "negomor671@xitudy.com",
    "school": "promma",
    "firstname": "aaaa",
    "lastname": "bbb",
    "enteredYear": "2560",
    "classYear": 3,
    "isActive": "active",
    "tel": "0800000000",   //optional
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
  "message": "Lorem Ipsum",
}
```
</TabItem>

</Tabs>