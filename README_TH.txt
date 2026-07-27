Production Organization System v15

เพิ่มจาก v14:
- Skill Matrix แยกตาม Section
- ทักษะเฉพาะแต่ละ Section (Stamping อ้างอิงโครงสร้างจากไฟล์ Stamping Deptment.xlsx)
- Skill Level 1-5 พร้อมสีแสดงระดับ
- Admin ปรับระดับรายทักษะได้
- วันที่อัปเดตล่าสุดและกำหนดอัปเดตครั้งถัดไปทุก 3 เดือน
- ตัวกรองผู้ที่ถึงกำหนด/เกินกำหนด
- สรุปจำนวนและเปอร์เซ็นต์พนักงาน Level 3 ขึ้นไป
- Skill Card รายบุคคล พร้อมรูป, เครื่องจักร, วันหมดรอบ และ QR
- พิมพ์ Skill Card รายคนหรือทั้ง Section
- พิมพ์ Skill Matrix ราย Section หรือทุก Section
- พิมพ์/PDF ได้ครบ: Organization, Section, Section Chart, รายชื่อพนักงาน, Training Plan, ข้อสอบ, รายการรอผล, ประวัติสอบ, Skill Matrix, Skill Card

วิธีติดตั้ง:
1. แตก ZIP
2. อัปโหลดไฟล์ทั้งหมดทับใน GitHub repository
3. นำ firestore.rules ไปวางใน Firebase Firestore Rules แล้วกด Publish
4. ตรวจ firebase-config.js ให้เป็นค่าเดิมของโปรเจกต์

การบันทึกเป็น PDF: กดปุ่มพิมพ์ แล้วเลือก Save as PDF / บันทึกเป็น PDF
