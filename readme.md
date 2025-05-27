# 🎯 แอปทดสอบเลขยกกำลัง (Exponent Quiz App)

แอปพลิเคชันสำหรับทดสอบความรู้เรื่องเลขยกกำลัง พัฒนาด้วย React พร้อมระบบจับเวลาและการตอบด้วยเสียง

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## ✨ Features

- 📝 **ข้อสอบ 20 ข้อ** พร้อมระบบให้คะแนน
- ⏱️ **ตัวจับเวลา** ปรับเวลาต่อข้อได้ (ค่าเริ่มต้น 5 วินาที)
- 🎤 **ตอบด้วยเสียง** รองรับทั้งภาษาไทยและอังกฤษ
- 📊 **บันทึกประวัติ** ดูผลสอบย้อนหลังได้
- 👥 **ระบบห้องเรียน** จัดการนักเรียนและห้องเรียนได้
- 📁 **นำเข้า/ส่งออกข้อมูล** รองรับไฟล์ JSON
- 🎨 **UI สวยงาม** ใช้งานง่าย Responsive Design

## 🚀 Demo

[ดูตัวอย่าง Demo](https://your-app-name.vercel.app)

## 📦 การติดตั้ง

### วิธีที่ 1: ใช้งานแบบ Static HTML
1. ดาวน์โหลด `index.html`
2. เปิดไฟล์ด้วย Web Browser
3. พร้อมใช้งานทันที!

### วิธีที่ 2: Deploy บน Vercel
1. Fork หรือ Clone repo นี้
2. ไปที่ [Vercel](https://vercel.com)
3. Import Git Repository
4. Deploy!

## 💻 การใช้งาน

### สำหรับครู/ผู้ดูแล
1. **เพิ่มห้องเรียน**: ไปที่ตั้งค่า → เพิ่มห้องเรียน
2. **เพิ่มนักเรียน**: ไปที่ตั้งค่า → เพิ่มนักเรียน
3. **นำเข้าข้อสอบ**: คลิก "นำเข้าข้อสอบ" → เลือกไฟล์ JSON
4. **ดูประวัติ**: คลิก "ดูประวัติ" เพื่อดูผลสอบทั้งหมด
5. **บันทึกข้อมูล**: คลิก "บันทึกข้อมูล" เพื่อ Export เป็น JSON

### สำหรับนักเรียน
1. เลือกห้องเรียนและชื่อตนเอง
2. คลิก "เริ่มทำข้อสอบ"
3. ตอบคำถามโดยพิมพ์หรือพูด
4. ดูผลคะแนนเมื่อทำเสร็จ

## 🎤 การใช้ Speech Recognition

### Browser ที่รองรับ:
- ✅ Google Chrome (แนะนำ)
- ✅ Microsoft Edge
- ✅ Safari (iOS/macOS)
- ❌ Firefox (ยังไม่รองรับ)

### วิธีใช้:
1. คลิกปุ่ม "พูดไทย" หรือ "พูดอังกฤษ"
2. อนุญาตการใช้ไมโครโฟน (ครั้งแรก)
3. พูดคำตอบ เช่น "แปด" หรือ "eight"
4. ระบบจะแปลงเป็นตัวเลขอัตโนมัติ

## 📄 รูปแบบไฟล์ JSON

### นำเข้าข้อสอบ:
```json
[
  {
    "id": 1,
    "question": "2³ = ?",
    "answer": "8",
    "points": 1
  },
  {
    "id": 2,
    "question": "5² = ?",
    "answer": "25",
    "points": 2
  }
]
```

### Export ข้อมูล:
ระบบจะ Export ข้อมูลทั้งหมดรวมถึง:
- ประวัติการสอบ
- รายชื่อนักเรียน
- รายชื่อห้องเรียน
- ชุดข้อสอบทั้งหมด

## 🛠️ การพัฒนาเพิ่มเติม

### เพิ่ม Database (Firebase):
```javascript
// ติดตั้ง Firebase
npm install firebase

// เพิ่มใน index.html
import { initializeApp } from 'firebase/app';
import { getDatabase } from 'firebase/database';
```

### Custom Styling:
- ใช้ Tailwind CSS
- แก้ไขได้ใน `<style>` tag

## 📱 Responsive Design

- **Desktop**: ✅ เต็มฟีเจอร์
- **Tablet**: ✅ ปรับขนาดอัตโนมัติ
- **Mobile**: ✅ ใช้งานได้ (Speech อาจไม่ stable)

## 🔧 Troubleshooting

| ปัญหา | วิธีแก้ |
|-------|--------|
| Speech ไม่ทำงาน | ใช้ Chrome/Edge/Safari และอนุญาต Microphone |
| ข้อมูลหาย | Export บ่อยๆ หรือใช้ Database |
| Deploy ไม่ได้ | ตรวจสอบชื่อไฟล์และ package.json |

## 📊 Performance

- **Load Time**: < 2 วินาที
- **Bundle Size**: ~500KB (รวม libraries)
- **Browser Support**: Modern browsers (ES6+)

## 🤝 Contributing

ยินดีรับ Pull Requests! กรุณา:
1. Fork the Project
2. Create your Feature Branch
3. Commit your Changes
4. Push to the Branch
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License.

## 👏 Credits

- React 18
- Tailwind CSS
- Font Awesome Icons
- Web Speech API

## 📞 Support

หากพบปัญหาหรือมีข้อเสนอแนะ:
- Open an Issue
- หรือติดต่อ: your-email@example.com

---

Made with ❤️ for Thai Students