---
sidebar_position: 1
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/data


ใช้สำหรับการดูข้อมูลส่วนตัวของแต่ละ User อีกทั้งยังให้ข้อมูลโรงเรียน ที่ user คนนั้นสังกัด และข้อมูลตาม role ของตนเอง ได้แก่ `system admin`, `school admin`, `teacher`, `student` โดยเราจะตรวจสอบ user ผ่าน Barear Token ที่ส่งมา 

**Method** `GET`

**Role ที่ใช้ได้** `system admin`, `school admin`, `teacher`, `student`

**content-type** `application/json`

<Tabs
  groupId="type"
  defaultValue="host"
  values={[
    { label: 'System admin', value: 'host', },
    { label: 'School Admin', value: 'admin', },
    { label: 'Teacher', value: 'teacher', },
    { label: 'Student', value: 'student', },
  ]
}>

<TabItem value="host">

```json title="Response"
{
  "success": true,
  "data_user": {
    "email": "barinschool@hotmail.com",
    "schoolID": "xxxx",
    "role": "host",
    "status": "Active"
  },
  "data_role": {
    "firstname": "barin",
    "lastname": "storm"
  },
  "data_school": {
    "schoolName": "xxxd",
    "paymentStatus": "pending",
    "status": "pending",
    "requests": [

    ],
    "clubs": [
      "631c6c83206c37ff705b2931",
      "631eed17f75f0547657bc097",
      "631eeb0d8cd1164e423f9d5f"
    ],
    "adminID": [

    ],
    "schedule": [
      {
        "schoolYear": 1995,
        "registerDate": "1996-10-29T20:24:00.000Z",
        "endOfRegisterDate": "1996-10-29T20:24:00.000Z",
        "endOfSchoolYear": "1996-10-29T20:24:00.000Z",
        "_id": "631f1504137efb85a40d7c35"
      },
      {
        "schoolYear": 1995,
        "registerDate": "1996-10-29T20:24:00.000Z",
        "endOfRegisterDate": "1996-10-29T20:24:00.000Z",
        "endOfSchoolYear": "1996-10-29T20:24:00.000Z",
        "_id": "63233d50328cc09ec9e6b24c"
      }
    ]
  }
}
```
</TabItem>

<TabItem value="admin">

```json title="Response"
{
  "success": true,
  "data_user": {
    "email": "tawanchai.ch@ku.th",
    "schoolID": "qwerty",
    "role": "admin",
    "status": "Active"
  },
  "data_role": {
    "tel": "0917893332"
  },
  "data_school": {
    "schoolName": "qwerty",
    "paymentStatus": "pending",
    "status": "pending",
    "requests": [

    ],
    "clubs": [

    ],
    "schedule": [

    ],
    "adminID": [

    ]
  }
}
```
</TabItem>

<TabItem value="teacher">

```json title="Response"
{
  "success": true,
  "data_user": {
    "email": "wedowa6500@edxplus.com",
    "schoolID": "qwerty",
    "role": "teacher",
    "status": "Active"
  },
  "data_role": {
    "firstname": "Champ",
    "lastname": "Chaisoro",
    "tel": "081111",
    "clubs": [

    ]
  },
  "data_school": {
    "schoolName": "qwerty",
    "paymentStatus": "pending",
    "status": "pending",
    "requests": [

    ],
    "clubs": [

    ],
    "schedule": [

    ],
    "adminID": [

    ]
  }
}
```
</TabItem>




<TabItem value="student">

```json title="Response"
{
  "success": true,
  "data_user": {
    "email": "tawanchai_champ@hotmail.com",
    "schoolID": "qwerty",
    "role": "student",
    "status": "Active"
  },
  "data_role": {
    "firstname": "Bird",
    "lastname": "tongchai",
    "enteredYear": 2021,
    "classYear": 3,
    "isActive": "Active",
    "clubs": [

    ]
  },
  "data_school": {
    "schoolName": "qwerty",
    "paymentStatus": "pending",
    "status": "pending",
    "requests": [

    ],
    "clubs": [

    ],
    "schedule": [

    ],
    "adminID": [

    ]
  }
}
```
</TabItem>

</Tabs>