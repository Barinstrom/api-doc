---
sidebar_position: 2
---

# /auth/:schoolID/addstudent


ใช้สำหรับการสร้าง user ที่มี role เป็น student ใน school ที่ระบุใน path parameter/variable :/school (หลายคน)โดยข้อมูลที่จะต้องส่งจะเป็น file csv (ข้อมูลที่อยู่ใน csv ของแต่ละคนจะเหมือนกับ request-body ของ addstudentone) และทำการส่ง activate token ไปทาง email ที่ได้ระบุไว้ โดยคนที่มีสิทธิ์การใช้จะมีเพียง user ที่มี role เป็น school admin ของโรงเรียนนั้น และ system admin เท่านั้น

**Method** `POST`


**Role ที่ใช้ได้** `school admin`, `system admin`


**content-type** `application/form-data`


**Request**

| key         | value       |
| ----------- | ----------- |
| Teachers    | csv file    |


```json title="Response"
{
  "success": true,
}
```