---
sidebar_position: 2
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /schools/approved


ใช้สำหรับการดึงทุกโรงเรียนที่ผ่านการ approve โดยสามารถที่จะ search ได้ด้วย

**Method** `GET`

**Role ที่ใช้ได้** `system admin`

**content-type** `application/json`

```json title="Request"
{
    "page" : number,
    "query" : {
      "schoolName": string,
    },
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
  ชื่อรร email
  
  [array list โรงเรียนทุกโรงเรียน ที่ approve]
}
```
</TabItem>

<TabItem value="fail">

```json title="Response"
{
  "success": false,
  "message": "Error cannot get data right now"
}
```
</TabItem>

</Tabs>




