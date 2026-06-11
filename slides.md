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
สารบัญรวมหัวข้อรายงานโครงงานวิจัย เพื่อง่ายต่อการค้นหาและเข้าชมเนื้อหา
<br>
<br>

1. Presentation Cover
2. What is Smart Web App Pen Test?
3. สารบัญ
4. Wabpentest
5. ภาพรวม
   - 1. หัวข้อการนำเสนอ

::right::

6. ส่วนที่ 1
   - 1. ที่มาและความสำคัญ
   - 2. วัตถุประสงค์และขอบเขต
   - 3. การแบ่งหน้าที่

<br>
 
7. ส่วนที่ 2

   - 1. ขั้นตอนดำเนินงาน
   - 2. สถาปัตยกรรมระบบ
   - 3. Workflow การสแกน
   - 4. วิธีตรวจช่องโหว่
   - 5. AI และการป้องกันข้อมูลหลุด
   - 6. การประเมินผล


---
layout: two-cols
layoutClass: gap-16
---

# สารบัญ

<br>

8. ส่วนที่ 3
   - 1. ซอฟต์แวร์และอุปกรณ์
   - 2. Technology Stack
   - 3. API และ Infrastructure
  
9. ส่วนที่ 4
   - 1. ความคืบหน้า
   - 2. สถานะล่าสุดของโครงงาน
   - 3. หลักฐานผลสแกนจริง
   - 4. หลักฐาน Unit Test

::right::

<br> <br> <br>

10. ส่วนที่ 5
   - 1. ชิ้นงาน
   - 2. หน้าจอหลักและการเลือก Module
   - 3. Dashboard รายงานผล
   - 4. รายละเอียดช่องโหว่
   - 5. AI Explanation
   - 6. แนวทางสาธิตหน้าห้อง
   - 7. ข้อจำกัดและแนวทางพัฒนาต่อ

<br>

11. สรุปผลโครงงาน


---
src: ./slides_part2.md
---