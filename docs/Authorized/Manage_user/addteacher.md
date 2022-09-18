---
sidebar_position: 4
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/add-teachers



ใช้สำหรับการสร้าง user ที่มี role เป็น teacher ใน school ที่ระบุใน path parameter/variable :/schoolID (หลายคน)โดยข้อมูลที่จะต้องส่งจะเป็น array ของ json(ข้อมูลของแต่ละ document ใน request-body ของ path /:schoolID/add-teacher)และทำการส่ง activate token ไปทาง email ที่ได้ระบุไว้ โดยคนที่มีสิทธิ์การใช้จะมีเพียง user ที่มี role เป็น school admin ของโรงเรียนนั้นๆ และ system admin เท่านั้น

**Method** `POST`


**Role ที่ใช้ได้** `school admin` , `system admin`


**content-type** `application/form-data`


```json title="Request"
[   
    {
        "email": "paradorn248@gmail.com",
        "firstname": "Erk",
        "lastname": "dont delete",
        "tel": "081111789",
    },
    {
        "email": "markpts03123456@gmail.com",
        "firstname": "Erk",
        "lastname": "dont delete",
        "tel": "081111",
    },
    {
        "email": "qaqwswderftrgpolikmnbvcx@gmail.com",
        "firstname": "Erk",
        "lastname": "dont delete",
        "tel": "081111",
    }
]
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