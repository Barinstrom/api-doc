---
sidebar_position: 2
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/add-students


API สำหรับการเพิ่ม student เข้าไปในระบบ โดยที่ทางฝั่ง frontend จะรับไฟล์ csv ที่มีข้อมูลของนักเรียนหลายๆ คน แล้วแปลงข้อมูลเป็น array of json โดย key ของ json แต่ละตัว ที่จำเป็นต้องใส่ จะเหมือนกับ endpoint `/:schoolID/add-student` ทุกประการ 

โดยหากระบบตรวจสอบพบว่า `email` ของนักเรียนที่ใส่เข้ามานั้นมีอยู่ในฐานข้อมูลอยู่แล้ว จะเป็นการ update ข้อมูลทับข้อมูลเก่าที่มีอยู่แทน

**Method** `POST`


**Role ที่ใช้ได้** `school admin`, `system admin`


**content-type** `application/่json`


```json title="Request"
[
  {
    "email": "tawanchai_champ@hotmail.com",
    "firstname": "Bird",
    "lastname": "tongchai",
    "enteredYear": "2021",
    "classYear": "3",
    "isActive": "Active"
  },
  {
    "email": "tawanchaichamps@gmail.com",
    "firstname": "To",
    "lastname": "Silly fools",
    "enteredYear": "2020",
    "classYear": "4",
    "isActive": "Active"
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
  "message": "Lorem Ipsum",
}
```
</TabItem>

</Tabs>