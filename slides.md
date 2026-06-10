---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://i0.wp.com/thetac.tech/wp-content/uploads/2024/10/TAC-Cybersecurity-Non-Profit-3.jpg?resize=800%2C366&ssl=1
# some information about your slides (markdown enabled)
title: Presentation Cover
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable Comark Syntax: https://comark.dev/syntax/markdown
comark: true
# duration of the presentation
duration: 35min
---

# Smart Web App Pen Test

<div @click="$slidev.nav.next" class="mt-12 py-1" hover:bg="white op-10">
  Press Space for next page <carbon:arrow-right />
</div>

<div class="abs-br m-6 text-xl">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="slidev-icon-btn">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out
---

# What is Smart Web App Pen Test?

 #### โครงงานนี้เป็นการศึกษาและออกแบบระบบวิเคราะห์ช่องโหว่ของซอร์สโค้ดโดยใช้ปัญญาประดิษฐ์ เพื่อช่วยให้การตรวจสอบความปลอดภัยของซอฟต์แวร์มีประสิทธิภาพมากขึ้น ขอบเขตของโครงงานครอบคลุมการศึกษาแนวคิดพื้นฐานที่เกี่ยวข้องกับการวิเคราะห์ช่องโหว่ของซอฟต์แวร์การออกแบบภาพรวม
 <br>

- 📝 **บทนํา** - ภาพรวมของตัวโครงงาน
- 🎨 **ระเบียบวิธีวิจัย** - ขั้นตอนตั้งแต่การออกแบบและเป้าหมายการพัฒนา
- 🤹 **สรุปความคืบหน้า** - สรุปความคืบหน้าทั้งหมดนับจากการนำเสนอครั้งล่าสุด
- 🎥 **ชิ้นงาน** - นำเสนอชิ้นงานที่สมบูรณ์แล้ว
<br>
<br>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
layout: two-cols
layoutClass: gap-16
---

# สารบัญ

```
uint_32t Payload = Malware + Insecure trust;
```
<br>
<br>
สารบัญรวมหัวข้อรายงานโครงงานวิจัย เพื่อง่ายต่อการค้นหาและเข้าชมเนื้อหา

::right::

<Toc text-sm minDepth="1" maxDepth="2" />

---
transition: fade-out
---

# บทนำ

 #### ปัจจุบันซอฟต์แวร์มีความซับซ้อนมากขึ้น ทำให้เกิดช่องโหว่ด้านความปลอดภัยได้ง่าย แม้ว่าจะมีเครื่องมือสำหรับตรวจสอบช่องโหว่ของซอร์สโค้ดอยู่แล้วแต่ส่วนใหญ่ยังใช้การตรวจสอบแบบกฎตายตัว ซึ่งไม่สามารถเข้าใจบริบทการทำงานของโค้ดได้ครบถ้วนและมักเกิดการแจ้งเตือนผิดพลาด
  
<br>

 #### โครงงานนี้จึงมีแนวคิดในการนำปัญญาประดิษฐ์มาประยุกต์ใช้ในการวิเคราะห์ช่องโหว่ของซอร์สโค้ด เพื่อเป็นแนวทางในการออกแบบระบบตรวจสอบความปลอดภัย ที่มีความเหมาะสมและมีประสิทธิภาพมากขึ้น
<br>

## ประโยชน์ที่คาดว่าจะได้รับ
- ได้ระบบตรวจสอบความปลอดภัยของซอร์สโค้ดแบบอัตโนมัติ 
ตามมาตรฐาน OWASP ที่ช่วยลดข้อผิดพลาดด้านความปลอดภัยของซอฟต์แว
- ได้แนวทางการประยุกต์ใช้ AI ในการวิเคราะห์ช่องโหว่
เชิงบริบท ที่มีความแม่นยำและลดการแจ้งเตือนที่ไม่ถูกต้อง
- นักศึกษามีความรู้และทักษะด้านการเขียนโปรแกรมอย่างปลอดภัยเพิ่มขึ้น จากการใช้งานระบบช่วยสอนพร้อมแนวทางการแก้ไข
ที่ถูกต้องในทางการพัฒนาระบบวิเคราะห์ช่องโหว่ของซอฟต์แวร์
ด้วย AI

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
transition: fade-out
---

# ระเบียบวิจัย

 ในการพัฒนาเว็บแอปพลิเคชัน Smart Web App Pentest สําหรับการทดสอบเจาะระบบ web app โดยเฉพาะ มี
วัตถุประสงค์หลักดังนี้

1. การออกแบบและสร้าง <br>
1.1 การสร้าง ออกแบบและพัฒนาเว็บแอปพลิเคชันสําหรับการทดสอบเจาะระบบที่รองรับการตรวจจับและวิเคราะห์
ช่องโหว่ตามมาตรฐานสากล OWASP Top 10 <br>
1.2 การประยุกต์เพื่อประยุกต์ใช้เทคโนโลยีโมเดลภาษาขนาดใหญ่ (LLMs) มาช่วยในการสร้าง Payload และวางกล
ยุทธ์การโจมตีแบบอัตโนมัติ 
2. เป้าหมายด้านการพัฒนา <br>
2.1 การพัฒนา เพื่อพัฒนาระบบคัดกรองช่องโหว่ทางทฤษฎีและลดอัตราการแจ้งเตือนที่ผิดพลาดให้เหลือน้อยที่สุด <br>
2.2 การระบุความแม่นยํา เพื่อประเมินประสิทธิภาพของระบบ ในด้านความสําเร็จของการค้นพบช่องโหว่ เปรียบเทียบ
กับเครื่องมือทดสอบมาตรฐานในปัจจุบัน และวิเคราะห์ความคุ้มค่าด้านทรัพยากรและเวลาที่ใช้ในการทดสอบ

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
transition: fade-out
---

# สรุปความคืบหน้า

 

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

---
src: ./slides_part2.md
---