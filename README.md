# รายงานแบบฝึกหัด Socket API & Docker (Assignment 1 & 2)

**ข้อมูลผู้จัดทำ**
* ชื่อ-นามสกุล: [osamu eguchi]
* รหัสนักศึกษา: [6814951032]
* กลุ่ม/เซคชัน: [1]

---

## 🛠️ แบบฝึกหัดที่ 1: ระบบ Chat ด้วย Docker (2 Clients & 1 Server)

### คำอธิบายการทำงาน
ระบบแชทนี้ประยุกต์ใช้ Socket API แบบ TCP ในการส่งข้อมูลระหว่าง Client 2 ตัว ผ่าน Server กลาง โดยรันอยู่ในรูปแบบของ Docker Multi-container และใช้ Docker Compose ในการจัดการ

### ขั้นตอนการเริ่มทำงาน (How to run)
1. เปิด Terminal และเข้าไปที่โฟลเดอร์แบบฝึกหัดที่ 1:
   ```bash
   cd networkPro-lab3-6814951032
<img width="1166" height="616" alt="Screenshot 2026-11-27 094949" src="https://github.com/user-attachments/assets/29a1a01a-c012-4634-996a-4f840afb1712" />



🌐 แบบฝึกหัดที่ 2: เว็บแอปพลิเคชัน Flask และ Socket Server

<img width="1917" height="1198" alt="Screenshot 2026-11-27 101540" src="https://github.com/user-attachments/assets/e1d9fe04-5577-41bd-86f6-4a36a1b0532f" />


คำอธิบายการทำงาน
แอปพลิเคชันหน้าเว็บพัฒนาด้วย Flask รับข้อความผ่านการกดส่งฟอร์ม (POST Method) จากนั้น Flask จะทำหน้าที่เป็น Client ส่งข้อความนั้นต่อไปยัง Socket Server เพื่อทำการสะท้อนข้อมูลกลับ (Echo) และแสดงผลบนหน้าเว็บ
เปิด Terminal และเข้าไปที่โฟลเดอร์แบบฝึกหัดที่ 2:
cd exercise-2
สั่งรัน Docker Compose:
docker-compose up --build
เปิดเว็บเบราว์เซอร์ไปที่ลิงก์: http://localhost:5000 เพื่อทำการทดสอบส่งข้อความ
🧹 วิธีการหยุดการทำงานและเคลียร์ Resources (สำหรับทั้งสองแบบฝึกหัด)
ใช้คำสั่งนี้ในโฟลเดอร์ที่มีไฟล์ docker-compose.yml:

docker-compose down

---

### 3. ขั้นตอนการนำโค้ดขึ้น GitHub (Git Commands)

1. **สร้าง Repository บนเว็บ GitHub**:
   * ไปที่ [GitHub](https://github.com) และล็อกอินเข้าสู่ระบบ
   * คลิกปุ่ม **New** เพื่อสร้าง Repository ใหม่ ตั้งชื่อเช่น `socket-docker-assignment` (แนะนำให้ตั้งค่าเป็น **Public** เพื่อให้อาจารย์เข้าถึงได้โดยไม่ต้องขออนุญาต)

2. **ผูกและอัปโหลดไฟล์ผ่าน Terminal เครื่องตนเอง**:
   เปิด Terminal ในโฟลเดอร์โปรเจกต์หลักของคุณ แล้วรันคำสั่งต่อไปนี้:
   ```bash
   # 1. เริ่มต้นใช้งาน Git ในโฟลเดอร์นี้
   git init

   # 2. แอดไฟล์ทั้งหมดเตรียมอัปโหลด
   git add .

   # 3. บันทึกประวัติ (Commit)
   git commit -m "Initial commit: socket programming assignment 1 & 2"

   # 4. เปลี่ยนชื่อสาขาหลักเป็น main
   git branch -M main

   # 5. เชื่อมต่อไปยัง GitHub Repository ที่เพิ่งสร้าง (แทนที่ URL ด้านล่างด้วยของคุณ)
   git remote add origin https://github.com/[ชื่อผู้ใช้ของคุณ]/[ชื่อ-repo-ของคุณ].git

   # 6. อัปโหลดโค้ดขึ้น GitHub
   git push -u origin main
