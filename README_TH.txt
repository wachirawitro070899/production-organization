วิธีเปิดให้คนอื่นดูและ Login ได้จริง

1) สร้าง Firebase Project ที่ console.firebase.google.com
2) เปิด Authentication > Sign-in method > Email/Password
3) สร้างบัญชี Admin ใน Authentication > Users
4) เปิด Firestore Database
5) นำค่า Firebase Config มาแทนในไฟล์ firebase-config.js
6) นำข้อความใน firestore.rules ไปวางที่ Firestore > Rules แล้วกด Publish
7) อัปโหลดไฟล์ index.html และ firebase-config.js ไปยัง GitHub Pages / Netlify / Firebase Hosting

สิทธิ์ในระบบ
- บุคคลทั่วไป: ดู Organization Chart, Section และค้นหาได้ โดยไม่ต้อง Login
- Admin: Login เพื่อเพิ่มและลบพนักงาน
- ข้อมูลเก็บใน Firestore ทำให้ทุกคนเห็นข้อมูลชุดเดียวกัน

หมายเหตุ: ต้องเปิดเว็บผ่าน Hosting หรือ local web server ไม่ควรดับเบิลคลิก file:// เพราะ ES Module และ Firebase อาจไม่ทำงาน


เวอร์ชัน v8: Admin สามารถแก้ไขรหัส ชื่อ เบอร์โทร วันที่เริ่มงาน Section และตำแหน่งได้จากหน้า Search โดยกดปุ่ม แก้ไขข้อมูล
