---
sidebar_position: 12
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# /:schoolID/get-review


ใช้เรียกข้อมูล review ทั้งหมด ของชุมนุมนั้น ๆ

**Method** `GET`

**Role ที่ใช้ได้** `system admin`, `school admin`, `teacher`, `student`

**content-type** `application/form-data`

**Request**

| key         | value       |
| ----------- | ----------- |
| page   | 1    |
| clubID   | 631c6c83206c37ff705b2931  |

<Tabs
  groupId="type"
  defaultValue="success"
  values={[
    { label: 'success', value: 'success', },
    { label: 'fail', value: 'fail', }
  ]
}>

<TabItem value="success">

```json title="Response (Parginate)"
{
    "docs": [
        {
            "_id": "631f11102576dc5a6f35431c",
            "textReview": "test test",
            "groupID": "1",
            "studentID": "631ed901cbc23688f173c15f",
            "__v": 0
        },
        {
            "_id": "631f1169d5dea5ea687d8bbd",
            "textReview": "test test",
            "groupID": "1",
            "studentID": "631ed901cbc23688f173c15f",
            "__v": 0
        },
        {
            "_id": "631f11a17ab817d554ef88be",
            "textReview": "test test",
            "groupID": "1",
            "studentID": "631ed901cbc23688f173c15f",
            "__v": 0
        }
    ],
    "totalDocs": 9,
    "limit": 3,
    "totalPages": 3,
    "page": 1,
    "pagingCounter": 1,
    "hasPrevPage": false,
    "hasNextPage": true,
    "prevPage": null,
    "nextPage": 2
}
```
</TabItem>

<TabItem value="fail">

```json title="Response"
{
  "error": "error message."
}
```
</TabItem>

</Tabs>


