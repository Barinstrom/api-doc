---
sidebar_position: 2
---

# /auth/:schoolID/setschedule


ใช้สำหรับการ update schedule ของ school (เวลาเริ่ม/สิ้นสุด การลงทะเบียนชุมนุม, เวลาจบปีการศึกษา)

**Method** `PUT`

**Role ที่ใช้ได้** `school admin` , `system admin`

**content-type** `application/json`

```json title="Request"
{
    "registerDate": "1995-6-17T03:24:00",
    "endOfRegisterDate": "1995-6-24T03:24:00",
    "endOfSchoolYear": "1996-10-30T03:24:00"
}
```

```json title="Response"
{
  "success": true
}
```