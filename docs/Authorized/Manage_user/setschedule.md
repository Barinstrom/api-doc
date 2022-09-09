---
sidebar_position: 11
---

# /:schoolID/set-schedule


ใช้สำหรับการ update schedule ของ school (เวลาเริ่ม/สิ้นสุด การลงทะเบียนชุมนุม, เวลาจบปีการศึกษา)

**Method** `PATCH`

**Role ที่ใช้ได้** `school admin` , `system admin`

**content-type** `application/json`

```json title="Request"
{
    "schoolYear": "1995",
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