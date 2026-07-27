PRODUCTION ORGANIZATION SYSTEM - VERSION 20

แก้ไขสำคัญ:
- รายชื่อพนักงานจากไฟล์ Excel จำนวน 116 คนจะแสดงทันทีบนหน้าเว็บ
- ไม่ต้องรอให้ Firestore มีข้อมูลก่อน
- หาก Firestore มีข้อมูลเดิม ระบบจะนำข้อมูลเดิม เช่น รูปและระดับ Skill มารวมกับรายชื่อ Excel
- ปุ่มอัปโหลดเข้า Firebase ยังใช้งานได้สำหรับ Admin

Production Organization System — Version 18

อัปเดต Header บริษัท:
- เพิ่มโลโก้ JINRONG
- เพิ่มชื่อบริษัท JINRONG ELECTRONIC TECHNOLOGY (THAILAND) COMPANY LIMITED
- ปรับ Header ให้รองรับคอมพิวเตอร์และโทรศัพท์
- คงระบบ Skill Matrix, Skill Card QR, Print และ Download PDF จาก Version 17

Production Organization Training v17

เพิ่มในเวอร์ชันนี้:
- หน้า QR Skill Matrix มีปุ่มพิมพ์แยกจากปุ่มดาวน์โหลด PDF
- ปุ่มดาวน์โหลดสร้างไฟล์ PDF โดยตรง ชื่อไฟล์อ้างอิงรหัสพนักงาน
- PDF แสดงเฉพาะข้อมูลพนักงานและ Skill Matrix ของ Section นั้น
- รองรับ A4 แนวนอน

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


Version 16
- QR Code บน Skill Card เปิดหน้าเฉพาะ Skill Matrix ของพนักงานคนนั้น
- แสดงเฉพาะทักษะของ Section ที่พนักงานสังกัด
- ซ่อนเมนู Organization, Training, Exam และข้อมูลพนักงานคนอื่น
- หน้า QR รองรับมือถือและพิมพ์/บันทึก PDF


VERSION 19 - EMPLOYEE IMPORT
- เพิ่มรายชื่อพนักงานจาก Excel จำนวน 116 คน ครบ 10 Section
- Admin เปิดหน้า Search แล้วกด 'อัปโหลดรายชื่อ 116 คนเข้า Firebase'
- ใช้รหัสพนักงานเป็น Document ID ป้องกันข้อมูลซ้ำ
- การอัปโหลดซ้ำจะอัปเดตข้อมูลพื้นฐานและเก็บรูป/Skill เดิมไว้
- ลบปุ่มเครื่องหมายบวกใต้ Organization Card
- Header เหลือเฉพาะชื่อบริษัทและชื่อระบบ


VERSION 21 - FIX LIVE DEPLOYMENT
- ฝังรายชื่อพนักงานใน index.html โดยตรง
- ฝังโลโก้ใน index.html โดยตรง
- รายชื่อยังแสดงแม้ Firebase/CDN เชื่อมต่อไม่ได้
- ZIP วางไฟล์ไว้ระดับราก พร้อมอัปโหลดขึ้น GitHub Pages
