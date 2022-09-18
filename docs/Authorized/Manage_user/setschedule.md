---
sidebar_position: 11
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/set-schedule


ใช้สำหรับการ update schedule ของ school (เวลาเริ่ม/สิ้นสุด การลงทะเบียนชุมนุม, เวลาจบปีการศึกษา)

**Method** `PATCH`

**Role ที่ใช้ได้** `school admin` , `system admin`

**content-type** `application/json`

|PATH variable |Descripton|
|-----|--------|
|schoolID|เลข ID ของแต่ละโรงเรียน |

```json title="Request"
{
    "schoolYear": "1995",
    "registerDate": "1995-6-17T03:24:00",
    "endOfRegisterDate": "1995-6-24T03:24:00",
    "endOfSchoolYear": "1996-10-30T03:24:00"
    
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
  "success": true
}
```
</TabItem>

<TabItem value="fail">

```json title="Response"
{
  "success": false,
  "message": "lorem ipsum."
}
```
</TabItem>

</Tabs>