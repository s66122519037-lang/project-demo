PROJECT DEMO: ระบบประเมินนักศึกษาฝึกงาน (Frontend)

This is a Next.js project bootstrapped with create-next-app.

Getting Started (Setup & Run)

เพื่อให้โปรเจกต์นี้ทำงานได้เต็มรูปแบบ คุณต้องตั้งค่าเชื่อมต่อกับระบบ Backend (Elysia.js) และฐานข้อมูล (MongoDB/Prisma) ก่อนเริ่ม Dev Server

1. Prerequisites (สิ่งที่ต้องมีก่อนเริ่ม)

ต่อไปนี้คือสิ่งที่โปรเจกต์ต้องการ:
```
Node.js (v20.x.x+)
npm หรือ bun

Backend Server (Project Demo Backend) ต้องไม่รันอยู่ที่ Port 3000 หรือซํ่ากับ Port ของฝั่งหน้าบ้าน  (โปรดตรวจสอบการตั้งค่า Port ในไฟล์ .env)
```
2. Installation (ติดตั้ง Dependencies)

หลังจาก Clone Repository นี้มาแล้ว ให้เข้าไปในโฟลเดอร์โปรเจกต์ และติดตั้ง Packages ทั้งหมด:
```
npm install
# หรือ
bun install
```

3. Environment Setup (เชื่อม Backend)

สร้างไฟล์ชื่อ .env ใน Root Directory ของโปรเจกต์ (ระดับเดียวกับ package.json) และกำหนด URL สำหรับเชื่อมต่อ API Backend:
```

# ----------------------------------------------------
# NEXT.JS FRONTEND CONFIG
# ----------------------------------------------------

# URL ของ Backend Server (Elysia.js) 
# ต้องเป็น Port เดียวกับที่ตั้งค่าใน Backend (แนะนำ 3001)
NEXT_PUBLIC_API_URL=http://localhost:3001

# ตัวอย่างสำหรับรัน Production
# NEXT_PUBLIC_API_URL=[https://api.yourdomain.com](https://api.yourdomain.com)
```

4. Run Development Server

เมื่อตั้งค่า Environment เสร็จแล้ว ให้รัน Dev Server:
```
bun dev
# หรือ
npm run dev
```

Open http://localhost:3000 with your browser to see the result.

The page auto-updates as you edit the files.

💡 โครงสร้างโค้ดสำคัญ

โครงสร้างไฟล์หลักของ Next.js App Router:

```
app/page.tsx: หน้าหลัก (Home Page) ของแอปพลิเคชัน
app/components/: ที่เก็บ Components ต่างๆ เช่น NavBar.tsx, Footer.tsx

```

Learn More

To learn more about Next.js, take a look at the following resources:

Next.js Documentation - learn about Next.js features and API.

Learn Next.js - an interactive Next.js tutorial.
