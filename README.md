# nuxt-ui-starter

โปรเจกต์ Nuxt 4 + Nuxt UI v3 พร้อมธีมแบบกำหนดเอง (ชุดสี custom-primary / custom-neutral, โหมดมืด, locale ภาษาไทย) พร้อมพัฒนาต่อทันที

## เริ่มต้น

```bash
npm install
npm run dev
```

เปิด http://localhost:3000 ในเบราว์เซอร์

## Deploy ไปยัง Vercel

1. Push รีโปนี้ขึ้น GitHub
2. ไปที่ https://vercel.com/new แล้ว import รีโปนี้
3. กด Deploy ระบบจะตรวจจับเป็นโปรเจกต์ Nuxt ให้อัตโนมัติ และออกโดเมน `.vercel.app` ให้

## โครงสร้าง

- `app/assets/css/main.css` — design tokens และชุดสีทั้งหมด แก้ไขสีที่นี่จุดเดียว
- `app/app.config.ts` — ชื่อแทนสี และ default variant ของคอมโพเนนต์ฟอร์ม
- `app/components/ColorModeToggle.vue` — ปุ่มสลับโหมดมืด/สว่าง
- `app/pages/index.vue` — หน้าตัวอย่างสำหรับตรวจสอบธีม
