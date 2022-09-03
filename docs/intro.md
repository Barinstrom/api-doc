---
sidebar_position: 1
slug: /
---

# API Intro

Let's discover **Barin API Documents.**.

## Getting Started

เริ่มต้นจากเราจะแบ่งประเภท API ออกเป็น 2 ประเภทใหญ่ๆ คือ
- `Unautorized` เป็น API ที่ไม่จำเป็นต้องมีการ login เข้ามาในระบบ ก็สามารถเรียกใช้ได้
- `Auth` เป็น API ที่จำเป็นต้องส่ง token ทุกครั้งที่ทำการ request กล่าวคือ ต้องมีการ login เพื่อ check role ของ user ด้วยว่ามีสิทธิ์เรียกใช้งาน endpoint ดังกล่าวหรือไม่ โดย endpoint ของ API ประเภทนี้จะขึ้นต้นด้วย `/auth` โดย roles ที่มีอยู่ในระบบจะมีอยู่ทั้งหมด 4 แบบ นั่นคือ
  - `host` หรือชื่อตามเอกสารคือ `System admin` มีสิทธิ์จัดการได้ทุกอย่างในระบบ
  - `admin` หรือชื่อตามเอกสารคือ `School admin` มีสิทธิ์ทั้งหมด **ภายในโรงเรียนของตนเอง**
  - `teacher` หรืออาจารย์ มีสิทธิ์ในการจัดการข้อมูลวิชาที่ตนเองเป็นผู้สอน
  - `student` หรือนักเรียน มีสิทธิ์ในการลงทะเบียนเรียน/ยกเลิกการลงทะเบียน รีวิวรายวิชาที่ผ่านมาแล้ว ภายในช่วงเวลาที่กำหนด

## Base URL

- [Staging](https://barin-backend-staging.herokuapp.com/) Function ค่อนข้างจะล่าสุดกว่า แต่อาจมี bug อยู่
- [Production](https://barin-backend.herokuapp.com/) Function ภายใน branch นี้ ยืนยันแล้วว่าสามารถใข้ได้จริง
 
