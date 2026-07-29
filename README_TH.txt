Production Organization Training v37

เพิ่มระบบ Evaluation Plan / Job Observation Plan
- นำเข้าแผนเดือนกรกฎาคม 2026 จากไฟล์ 07-2026.xlsx: CNC, Bending, Stamping, Welding
- กรอง Section, สถานะ, เดือน และค้นหาพนักงาน
- เพิ่มแผนสำหรับพนักงานซัพเข้าใหม่, ซัพปรับประจำ, ประเมินประจำ, Skill Upgrade และ Re-evaluation
- Job Observation Check Sheet 19 หัวข้อ
- คำนวณคะแนนอัตโนมัติ ผ่านเมื่อคะแนนไม่น้อยกว่า 80% และไม่มี Critical Safety Fail
- แสดงสถานะ Planned, Completed, Failed, Overdue
- เก็บข้อมูลใน Local Storage และรองรับการพิมพ์/PDF

Production Organization Training Version 36

เพิ่มระบบล็อกชุดข้อสอบตาม Skill Matrix เดิม
- ระบบอ่าน Level ต่ำสุดจากหัวข้อ Skill Matrix เดิม เพื่อกำหนดชุดข้อสอบ
- Level 1 -> Level 2 ใช้ Q1 Foundation Test
- Level 2 -> Level 3 ใช้ Q2 Operation Qualification
- Level 3 -> Level 4 ใช้ Q3 Advanced Operator
- Level 4 -> Level 5 ใช้ Q4 Trainer & Expert
- Level 5 ใช้ Q4 Renewal
- ยังไม่ครบกำหนด 3 เดือน: ปุ่มเริ่มสอบและพิมพ์ถูกล็อก
- ไม่มีประวัติประเมินเดิม: อนุญาตให้ประเมินครั้งแรกทันที
- หัวข้อ Practical Test ล็อกจากหัวข้อที่มี Level ต่ำสุดใน Matrix เดิม
- บันทึก Snapshot Skill เดิมก่อนปรับใหม่
- Level 4-5 ต้องรอ Admin อนุมัติ
- ผลสอบไม่ผ่านจะไม่สามารถปรับ Level สูงขึ้น

วิธีติดตั้ง: อัปโหลดไฟล์ทั้งหมดทับ Repository เดิม แล้วกด Ctrl+F5


Version 36 เพิ่ม Dropdown มาตรฐาน:
- ผู้ประเมินและผู้อนุมัติ
- เครื่องจักร/พื้นที่ประจำตาม Section
- หัวข้อทักษะตาม Skill Matrix ของ Section
- สัญชาติ ประเภทสัญญา เพศ ตำแหน่ง Section และตัวกรองต่าง ๆ
- ช่องที่เป็นข้อมูลเฉพาะ เช่น ชื่อ รหัส เบอร์โทร วันที่ คะแนน และหมายเหตุ ยังคงเป็นช่องกรอกตามความเหมาะสม


Version 38: ปรับ Dropdown รายชื่อพนักงาน ผู้ประเมิน และผู้อนุมัติทุกหน้าให้พิมพ์ค้นหาชื่อ/รหัสได้ พร้อมรองรับคีย์บอร์ดและรายชื่อที่โหลดภายหลังจาก Firebase


Version 39
- Dropdown พนักงานทุกหน้าดึงข้อมูลจาก Organization/Employees
- ต้องเลือก Section ก่อน แล้วจะแสดงเฉพาะพนักงานของ Section นั้น
- รองรับ Evaluation Plan, Online Examination, Employee Skill Card และ Skill Matrix Examination
- เพิ่มช่อง Section ในหน้า Skill Matrix Examination
- Dropdown รายชื่อยังสามารถพิมพ์ค้นหาชื่อหรือรหัสพนักงานได้
