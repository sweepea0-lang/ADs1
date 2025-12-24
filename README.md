# Ads Monitor Dashboard

เว็บกรอกข้อมูลตรวจสอบการยิงแอด  
คำนวณ "ยอดคุ้มค่าแอด" และส่งข้อมูลเข้า Google Sheet อัตโนมัติ

## สูตรที่ใช้
- ยอดคุ้มค่าแอด = ฝากแรก - ค่าบูท
- % คุ้มค่าแอด = ยอดคุ้มค่าแอด / ค่าแอด

## วิธีใช้งาน
1. สร้าง Google Sheet ชื่อ `Daily_Ads`
2. ใส่หัวคอลัมน์:
   date | campaign | adCost | firstDeposit | boothCost | adValue | pct | mtdPct | status | note | createdAt
3. วาง `Code.gs` ใน Apps Script แล้ว Deploy เป็น Web App
4. นำ Web App URL ไปใส่ใน `index.html`
5. เปิด `index.html` → กรอกข้อมูล → กดส่ง

## Deploy หน้าเว็บ
- ใช้ GitHub Pages / Vercel / Netlify
