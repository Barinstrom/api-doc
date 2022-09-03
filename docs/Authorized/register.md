---
sidebar_position: 1
---

# /register


ใช้สำหรับการสมัคร `School admin`


**Method** `POST`

**content-type** `application/json`

```json title="Request"
{
    "email": "negomor671@xitudy.com",
    "password": "champ",
    "confirmPassword": "champ",
  	"schoolID": "promma",
  	"schoolName": "Prommanusorn Phetchaburi",
    "certificate_doc": base64_string
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

