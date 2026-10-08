# Souksavanh Viengsavanh — Portfolio

เว็บไซต์ Portfolio โทนเหลือง–ดำ พร้อมรูปโปรไฟล์ ทักษะ ประวัติการเรียน และช่องทาง Facebook, Email, LinkedIn และโทรศัพท์

HTML, CSS, JavaScript, รูปโปรไฟล์ และฟอนต์ที่ใช้แสดงหัวข้อ รวมอยู่ใน `index.html` ไฟล์เดียว ไม่มีขั้นตอน build และไม่ต้องติดตั้ง npm

## เปิดในเครื่อง

แตก ZIP แล้วดับเบิลคลิก `index.html` เพื่อเปิดในเบราว์เซอร์

## อัปโหลดและเปิดเว็บด้วย GitHub Pages

1. ลงชื่อเข้าใช้ GitHub แล้วสร้าง repository ใหม่ เช่น `souksavanh-portfolio` เลือก **Public** สำหรับการใช้งาน GitHub Free
2. ใน repository เลือก **Add file → Upload files** แล้วอัปโหลดไฟล์และโฟลเดอร์ที่อยู่ภายใน ZIP หลังแตกไฟล์ อย่าอัปโหลด ZIP โดยตรง
3. ตรวจว่า `index.html` อยู่ระดับแรกของ repository ไม่ได้อยู่ภายในโฟลเดอร์ `github-package` หรือโฟลเดอร์ชื่ออื่น จากนั้นกด **Commit changes**
4. เปิด **Settings → Pages**
5. ใน **Build and deployment** ตั้งค่า **Source: Deploy from a branch**
6. ตั้งค่า **Branch: main** และโฟลเดอร์ **/(root)** แล้วกด **Save** ถ้า repository ใช้ชื่อ branch อื่น ให้เลือก branch ที่เก็บ `index.html` แทน
7. รอจนการเผยแพร่สำเร็จ แล้วเปิดลิงก์ที่ GitHub แสดงในหน้า Pages

ตัวอย่างรูปแบบ URL: `https://YOUR-USERNAME.github.io/souksavanh-portfolio/`

แทน `YOUR-USERNAME` ด้วยชื่อบัญชี GitHub ของคุณ และเปลี่ยนชื่อส่วนท้ายให้ตรงกับชื่อ repository

ไฟล์ `.nojekyll` ช่วยให้เผยแพร่เป็นเว็บ static โดยตรง หากระบบอัปโหลดข้ามไฟล์นี้ คุณสามารถสร้างไฟล์ชื่อ `.nojekyll` ใน repository ผ่าน **Add file → Create new file** ได้

เมื่อแก้ไข `index.html` และ commit ไปยัง branch ที่ตั้งไว้ GitHub Pages จะเผยแพร่ฉบับใหม่

## แก้ไขข้อมูล

เปิด `index.html` ใน VS Code แล้วค้นหาข้อความที่ต้องการแก้ไข

- เนื้อหาเว็บอยู่ภายใน `<body>`
- สี ระยะห่าง ฟอนต์ และรูปแบบมือถืออยู่ภายใน `<style>`
- โทนสีหลักตั้งไว้ที่ `--yellow`, `--black` และ `--white`
- เบอร์โทรใช้ `tel:0834216230` อยู่ทั้งส่วน Contact และ Footer
- ลิงก์ Facebook, LinkedIn และ Email ใช้ช่องทางจริงที่ระบุไว้
- ส่วน Projects ยังระบุว่ากำลังเตรียมผลงานแรก
- รูปและฟอนต์ฝังด้วย data URL จึงไม่มีปัญหาที่อยู่ไฟล์เมื่อใช้ URL ของ repository

## ไฟล์ในชุดนี้

| ไฟล์ | หน้าที่ |
| --- | --- |
| `index.html` | เว็บไซต์ทั้งหมด เปิดดูได้ทันที |
| `.nojekyll` | กำหนดให้ GitHub Pages เผยแพร่ไฟล์ static |
| `.gitignore` | ข้ามไฟล์ชั่วคราวของเครื่อง |
| `README.md` | วิธีเปิดเว็บ อัปโหลด และแก้ไข |
| `vendor/nimbus-sans/` | ต้นฉบับและประกาศสิทธิ์ของฟอนต์ที่ฝังไว้ |

## ถ้าเปิดเว็บแล้วเจอ 404

- ตรวจว่าไฟล์ชื่อ `index.html` เป็นตัวพิมพ์เล็ก และอยู่ที่ root ของ repository
- ตรวจว่า Pages เลือก branch ที่เก็บไฟล์นี้ และเลือก `/(root)`
- ดูผลการเผยแพร่ในแท็บ **Actions** และเปิด URL จากหน้า **Settings → Pages** หลังงานสำเร็จ

## เอกสารอ้างอิง

- [ตั้งค่าแหล่งเผยแพร่ GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [สร้างเว็บไซต์ GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)

ยังไม่ได้อัปโหลดไฟล์หรือเผยแพร่ไปยังบัญชี GitHub ของคุณ ชุดนี้พร้อมสำหรับนำไปอัปโหลดตามขั้นตอนด้านบน
