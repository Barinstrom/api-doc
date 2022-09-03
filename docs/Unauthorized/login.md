---
sidebar_position: 2
---

# /login


ใช้สำหรับการ login สำหรับทุก user

**Method** `POST`

**content-type** `application/json`

```json title="Request"
{
    "email": "negomor671@xitudy.com",
    "password": "champ"
}
```

```json title="Response"
{
  "success": true,
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJfaWQiOiI2MzEzMTYxMDVhNjRiNWJhODBkZDg2NzEiLCJlbWFpbCI6Im1hc2lkaXY5OTlAeGl0dWR5LmNvbSIsInNjaG9vbCI6ImhvcndhbmciLCJyb2xlIjoiYWRtaW4iLCJzdGF0dXMiOiJBY3RpdmUiLCJfX3YiOjAsImlhdCI6MTY2MjE5ODY1NiwiZXhwIjoxNjYyMjAyMjU2fQ.iTOxD59q1pdJQIeaWMU27qixLPhGNqCotNB-F-n1ZU8"
}
```