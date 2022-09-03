---
sidebar_position: 2
---

# /auth/:schoolID/deleteClub


ใช้สำหรับการลบข้อมูล club ที่เราต้องการจะลบใน school ที่ระบุใน parameter :/school ตั้งแต่ 1 club ขึ้นไป โดยคนที่มีสิทธิ์การใช้จะมีเพียง user ที่มี role เป็น school admin ของโรงเรียนที่ club นั้นอยู่และ system admin เท่านั้น

**Method** `POST`


**Role ที่ใช้ได้** `school admin, system admin`


**content-type** `application/json`

```json title="Request"
{
    "clubIDs": [...clubID],
}
```

```json title="Response"
{
  "success": true,
}
```