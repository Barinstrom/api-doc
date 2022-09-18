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
  "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJfaWQiOiI2MzFjNTEyMGU5YTk0NDc3Y2E4ZjRhNDAiLCJlbWFpbCI6ImJhcmluc2Nob29sQGhvdG1haWwuY29tIiwic2Nob29sSUQiOiJ4eHh4Iiwicm9sZSI6Imhvc3QiLCJzdGF0dXMiOiJBY3RpdmUiLCJjb25maXJtYXRpb25Db2RlIjoiYzBmNnl0clhVNDJBRnlqQXRaakxya2JpSCIsIl9fdiI6MCwicmVzZXRUb2tlbiI6ImV5SmhiR2NpT2lKSVV6STFOaUlzSW5SNWNDSTZJa3BYVkNKOS5leUpsYldGcGJDSTZJbUpoY21sdWMyTm9iMjlzUUdodmRHMWhhV3d1WTI5dElpd2lhV0YwSWpveE5qWXpNVEkyTkRreExDSmxlSEFpT2pFMk5qTXhNamN6T1RGOS5MX2k1UFdnYS1vT2ZBaDZLNTh1c3g4aEgtV01IUGVmY21QdWFVQm8wc3RrIiwiaWF0IjoxNjYzNDgyMDY5LCJleHAiOjE2NjM0ODU2Njl9.ECdUcXCR2hbUGDjrsc6JJjt5P0aVuln9BE9jIOdyAmE",
  "schoolID": "xxxx",
  "role": "host"
}
```