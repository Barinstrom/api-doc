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
  "data": {
    "email": "negomor671@xitudy.com",
    "school": "promma",
    "password": "$2a$10$AFnxU5sCXeuHCljSDDNviePPrl17OIuhpKQuen7t13xuqwFeafYQm",
    "role": "admin",
    "status": "Pending",
    "confirmationCode": "vXJTtyZGDZMmputizRX2qr4ew",
    "_id": "6310c1835c4f87dc9e92875a",
    "__v": 0
  }
}
```