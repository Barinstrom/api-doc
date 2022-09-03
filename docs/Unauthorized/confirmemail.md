---
sidebar_position: 3
---

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /confirm/:confirmationCode



ใช้สำหรับการยืนยัน email สำหรับ  `teacher` และ `student`

**Method** `GET`

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
  "message": "Activate finish",
}
```
</TabItem>

<TabItem value="fail">

```json title="Response"
{
  "message": "User Not found.",
}
```
</TabItem>

</Tabs>