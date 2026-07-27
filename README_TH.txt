Production Organization System v10

แก้ไขปัญหาปุ่ม "แก้ไขข้อมูล" กดไม่ได้ โดยเปลี่ยนจาก inline onclick
เป็นระบบ event listener ที่รองรับ Firebase Document ID และเบราว์เซอร์บน GitHub Pages

วิธีอัปเดต
1. แตกไฟล์ ZIP
2. อัปโหลดไฟล์ทั้งหมดทับไฟล์เดิมใน GitHub repository
3. กด Commit changes
4. รอ GitHub Pages อัปเดต 1-2 นาที
5. เปิดเว็บแล้วกด Ctrl + F5
6. ตรวจสอบว่าหัวเว็บแสดง v10 Edit Employee Click Fixed


V11 เพิ่ม Training Plan รายไตรมาส, Annual Training และ Skill Matrix Examination
กรุณาอัปเดต firestore.rules และกด Publish เพื่อให้บันทึกผลสอบได้


Version 12 เพิ่ม:
- Online Examination Q1-Q4 รวม 40 ข้อ
- ตรวจคะแนนอัตโนมัติ
- Practical Test / Job Observation ตาม Section และไตรมาส
- บันทึกประวัติผลสอบและ Skill Level
- เกณฑ์ผ่านข้อเขียน 80% และภาคปฏิบัติผ่านทุกข้อ
