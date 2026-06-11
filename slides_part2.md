---
class: px-14 py-10
transition: slide-left
---

# Webpentest

## ระบบตรวจสอบช่องโหว่เว็บไซต์ พร้อม AI อธิบายผลแบบ Local LLM

<div class="grid grid-cols-[1.05fr_.95fr] gap-8 mt-6 items-start">
  <div>
    <p class="text-sm text-blue-600 font-bold">โครงงานจบระดับปริญญาตรี</p>
    <h3>แนวคิดของโครงงาน</h3>
    <p class="text-lg">
      รวมการสแกนช่องโหว่เว็บ การจัดหมวดตาม OWASP Top 10 และ AI อธิบายผลภาษาไทยไว้ในระบบเดียว
      โดยใช้ AI local เพื่อลดความเสี่ยงข้อมูลหลุด
    </p>
    <div class="grid grid-cols-4 gap-4 mt-8">
      <div class="border-l-4 border-cyan-500 pl-3"><div class="text-4xl font-bold">5</div><div class="text-xs uppercase">Findings</div></div>
      <div class="border-l-4 border-emerald-500 pl-3"><div class="text-4xl font-bold">12</div><div class="text-xs uppercase">Tests OK</div></div>
      <div class="border-l-4 border-violet-500 pl-3"><div class="text-4xl font-bold">Local</div><div class="text-xs uppercase">AI Mode</div></div>
      <div class="border-l-4 border-amber-500 pl-3"><div class="text-4xl font-bold">A05</div><div class="text-xs uppercase">Main Risk</div></div>
    </div>
    <div class="mt-8 text-sm opacity-70">Penetration Tester | AI Developer / Engineer | Privacy by Default</div>
    <div class="text-sm opacity-70">วันที่จัดทำ: 10 มิถุนายน 2026</div>
  </div>
  <div class="rounded border overflow-hidden bg-white">
    <img src="./images/image-1-1.png" alt="Webpentest system screenshot" style="width:100%; display:block;" />
  </div>
</div>

---
class: px-14 py-10
---

# ภาพรวม

## สรุปโครงงานใน 1 นาที

<p class="opacity-70">อธิบายปัญหา แนวทางแก้ และผลลัพธ์ให้กรรมการเข้าใจเร็ว</p>

<div class="grid grid-cols-3 gap-5 mt-8">
  <div class="border rounded p-5">
    <h3 class="text-rose-600">ปัญหา</h3>
    <ul>
      <li>ผลสแกนอ่านยากสำหรับผู้เริ่มต้น</li>
      <li>ต้องใช้หลายเครื่องมือแยกกัน</li>
      <li>การส่งข้อมูลให้ AI ภายนอกมีความเสี่ยง</li>
    </ul>
  </div>
  <div class="border rounded p-5">
    <h3 class="text-blue-600">แนวทางแก้</h3>
    <ul>
      <li>Web UI สำหรับสแกนและดูรายงาน</li>
      <li>จัดหมวดตาม OWASP Top 10</li>
      <li>ใช้ Ollama local อธิบายผล</li>
    </ul>
  </div>
  <div class="border rounded p-5">
    <h3 class="text-emerald-600">ผลลัพธ์</h3>
    <ul>
      <li>พบ finding จริง 5 รายการ</li>
      <li>Unit test ผ่าน 12 เคส</li>
      <li>มี screenshot และ JSON evidence</li>
    </ul>
  </div>
</div>

<div class="mt-8 border-l-4 border-cyan-500 pl-5">
ประโยคสรุป: Wabpentest ช่วยให้การตรวจช่องโหว่เบื้องต้นและการสื่อสารวิธีแก้ทำได้เร็วขึ้น โดยคำนึงถึงความปลอดภัยของข้อมูล
</div>

---
class: px-14 py-10
---

## หัวข้อการนำเสนอ

<p class="opacity-70">เรียงตามรูปแบบที่ใช้ส่งโครงงานจบ</p>

<div class="grid grid-cols-5 gap-4 mt-10 text-sm">
  <div class="border-t-4 border-cyan-500 pt-4"><div class="text-3xl font-bold">01</div><h3>บทนำ</h3><p>ภาพรวมโครงงาน เป้าหมาย ขอบเขต และบทบาท</p></div>
  <div class="border-t-4 border-emerald-500 pt-4"><div class="text-3xl font-bold">02</div><h3>วิธีดำเนินโครงงาน</h3><p>ขั้นตอนออกแบบ พัฒนา ทดสอบ และประเมินผล</p></div>
  <div class="border-t-4 border-violet-500 pt-4"><div class="text-3xl font-bold">03</div><h3>ซอฟต์แวร์และอุปกรณ์</h3><p>เทคโนโลยี เครื่องมือ และสภาพแวดล้อมที่ใช้</p></div>
  <div class="border-t-4 border-amber-500 pt-4"><div class="text-3xl font-bold">04</div><h3>ความคืบหน้า</h3><p>สิ่งที่เสร็จแล้ว พร้อมหลักฐานและผลทดสอบ</p></div>
  <div class="border-t-4 border-rose-500 pt-4"><div class="text-3xl font-bold">05</div><h3>ชิ้นงาน</h3><p>สาธิตหน้าจอจริง ผลสแกนจริง และ AI explanation</p></div>
</div>

---
layout: center
class: text-center
---

# ส่วนที่ 1

## บทนำ

ภาพรวมของตัวโครงงาน

---
class: px-14 py-10
---

## ที่มาและความสำคัญ

<p class="opacity-70">ระบบเว็บต้องการทั้งการตรวจช่องโหว่และการอธิบายผลที่นำไปแก้ไขได้</p>

<div class="grid grid-cols-3 gap-5 mt-8">
  <div><h3>ปัญหาที่พบ</h3><ul><li>ช่องโหว่มักเกิดจาก header, cookie, config และ input</li><li>ผลจาก scanner มีศัพท์เทคนิคจำนวนมาก</li><li>ผู้พัฒนาต้องแปลผลเองก่อนเริ่มแก้ไข</li></ul></div>
  <div><h3>แนวคิดของระบบ</h3><ul><li>รวม UI, scanner, report และ AI ใน workflow เดียว</li><li>ใช้ OWASP Top 10 เป็นมาตรฐานกลาง</li><li>แสดงหลักฐานที่พบจริง ไม่ใช่รายงานลอย ๆ</li></ul></div>
  <div><h3>คุณค่าของโครงงาน</h3><ul><li>ช่วยเรียนรู้ web security</li><li>ช่วยผู้พัฒนาเข้าใจ impact และ remediation</li><li>ลดความเสี่ยงจากการส่งข้อมูลช่องโหว่ไป AI ภายนอก</li></ul></div>
</div>

---
class: px-14 py-10
---

## วัตถุประสงค์และขอบเขต

<p class="opacity-70">กำหนดเป้าหมายให้วัดผลได้และใช้งานอย่างรับผิดชอบ</p>

<div class="grid grid-cols-2 gap-5 mt-8">
  <div class="border rounded p-5"><h3>1. สร้างระบบสแกนช่องโหว่</h3><p>รับ URL เลือก module ติดตาม progress และดูรายงานได้</p></div>
  <div class="border rounded p-5"><h3>2. จัดหมวดตาม OWASP Top 10</h3><p>ช่วยให้รายงานมีมาตรฐานและตรวจสอบซ้ำได้</p></div>
  <div class="border rounded p-5"><h3>3. เพิ่ม AI อธิบายภาษาไทย</h3><p>อธิบาย impact, scenario, remediation และ verification</p></div>
  <div class="border rounded p-5"><h3>4. ป้องกันข้อมูลหลุด</h3><p>ใช้ Ollama local และ redact ข้อมูลสำคัญก่อนเข้า prompt</p></div>
</div>

<div class="mt-6 border-l-4 border-amber-500 pl-5">
ขอบเขตการใช้งาน: ใช้สำหรับเว็บไซต์ที่ผู้ใช้มีสิทธิ์ทดสอบเท่านั้น ผล automated scan เป็นข้อมูลตั้งต้นและต้องยืนยันซ้ำโดยผู้เชี่ยวชาญ
</div>

---
class: px-14 py-10
---

## การแบ่งหน้าที่

<p class="opacity-70">แยกบทบาทตามงานจริงของโครงงาน</p>

<div class="grid grid-cols-2 gap-8 mt-8">
  <div>
    <h3 class="text-cyan-600">1. Penetration Tester</h3>
    <ul><li>กำหนด scope และ target ที่ได้รับอนุญาต</li><li>ออกแบบขั้นตอนสแกนตาม OWASP Top 10</li><li>ตรวจ evidence, risk และ confidence</li><li>ยืนยันผลที่พบและจัดลำดับความเสี่ยง</li><li>สรุป remediation และ retest หลังแก้ไข</li></ul>
  </div>
  <div>
    <h3 class="text-violet-600">2. AI Developer / Engineer</h3>
    <ul><li>เชื่อม Ollama API และเลือก local model</li><li>ออกแบบ prompt ให้ตอบภาษาไทยและเน้นวิธีแก้</li><li>ทำ redaction ก่อนส่งข้อมูลเข้าโมเดล</li><li>ปิด external AI เป็นค่าเริ่มต้น</li><li>ทดสอบ error handling และ privacy logic</li></ul>
  </div>
</div>

---
layout: center
class: text-center
---

# ส่วนที่ 2

## วิธีดำเนินโครงงาน

ขั้นตอนตั้งแต่การออกแบบและเป้าหมายการพัฒนา

---
class: px-14 py-10
---

## ขั้นตอนดำเนินงาน


<p class="opacity-70">พัฒนาแบบเป็นลำดับ ตั้งแต่ศึกษามาตรฐานจนถึงตรวจผลจริง</p>

<div class="grid grid-cols-5 gap-3 mt-8 text-center">
  <div class="border rounded p-4"><div class="text-3xl font-bold">1</div><h3>ศึกษา</h3><p>OWASP, DAST, ZAP, LLM</p></div>
  <div class="border rounded p-4"><div class="text-3xl font-bold">2</div><h3>ออกแบบ</h3><p>workflow + architecture</p></div>
  <div class="border rounded p-4"><div class="text-3xl font-bold">3</div><h3>พัฒนา</h3><p>UI, API, scanner, AI</p></div>
  <div class="border rounded p-4"><div class="text-3xl font-bold">4</div><h3>ทดสอบ</h3><p>unit + real scan</p></div>
  <div class="border rounded p-4"><div class="text-3xl font-bold">5</div><h3>ประเมิน</h3><p>evidence + limitations</p></div>
</div>

<div class="grid grid-cols-2 gap-6 mt-8">
  <div><h3>หลักการออกแบบ</h3><p>ผู้ใช้ต้องกดสแกนง่าย แต่รายงานต้องมีข้อมูลเพียงพอสำหรับการแก้ไขจริง เช่น URL, method, evidence, risk และ solution</p></div>
  <div><h3>หลักการประเมินผล</h3><p>ประเมินจากผล API จริง screenshot จริง และ unit tests ของ scanner, OWASP mapping และ AI privacy</p></div>
</div>

---
class: px-14 py-10
---

## สถาปัตยกรรมระบบ

<p class="opacity-70">แยกชั้น UI, API, Scanner และ AI เพื่อให้ต่อยอดได้ง่าย</p>

<div class="grid grid-cols-4 gap-4 mt-8 text-center">
  <div class="border rounded p-4"><h3>Web UI</h3><p>HTML/JS</p></div>
  <div class="border rounded p-4"><h3>FastAPI</h3><p>scan/status/explain</p></div>
  <div class="border rounded p-4"><h3>Celery</h3><p>async worker</p></div>
  <div class="border rounded p-4"><h3>Baseline</h3><p>local fallback</p></div>
  <div class="border rounded p-4"><h3>OWASP ZAP</h3><p>full DAST</p></div>
  <div class="border rounded p-4"><h3>Report</h3><p>OWASP mapping</p></div>
  <div class="border rounded p-4 col-span-2"><h3>Ollama</h3><p>local LLM</p></div>
</div>

<div class="mt-8 border-l-4 border-cyan-500 pl-5">
เมื่อ ZAP/Celery พร้อม ระบบใช้ full scan; เมื่อไม่พร้อม ระบบยังสแกนพื้นฐานได้ด้วย baseline scanner เพื่อให้ demo และการทดสอบในเครื่องทำงานได้ต่อเนื่อง
</div>

---
class: px-14 py-10
---

## Workflow การสแกน

<p class="opacity-70">ลำดับการทำงานตั้งแต่ผู้ใช้กดสแกนจนถึงรายงานผล</p>

<div class="grid grid-cols-3 gap-4 mt-8">
  <div class="border rounded p-4"><h3>1 Input</h3><p>ตรวจ URL และ module ที่เลือก</p></div>
  <div class="border rounded p-4"><h3>2 Task</h3><p>เลือก engine: ZAP หรือ baseline</p></div>
  <div class="border rounded p-4"><h3>3 Discover</h3><p>โหลดหน้าและค้นหา URL ภายใน host</p></div>
  <div class="border rounded p-4"><h3>4 Detect</h3><p>ตรวจ header, cookie, exposed file, reflection หรือ ZAP alert</p></div>
  <div class="border rounded p-4"><h3>5 Normalize</h3><p>จัด risk, confidence และ OWASP category</p></div>
  <div class="border rounded p-4"><h3>6 Report</h3><p>แสดงผลและเปิด AI explanation</p></div>
</div>

---
class: px-14 py-10
---

## วิธีตรวจช่องโหว่

<p class="opacity-70">ระบบมีทั้ง baseline scanner ในตัวและ full scan ผ่าน OWASP ZAP</p>

<div class="grid grid-cols-2 gap-8 mt-8">
  <div>
    <h3>Baseline Scanner</h3>
    <ul><li>ใช้เมื่อไม่มี Celery/ZAP worker</li><li>ร้องขอ target URL จริงด้วย requests.Session</li><li>ตรวจ security headers, cookies, exposed files และ reflected parameters</li><li>จัด risk และ mapping OWASP จากหลักฐานที่พบ</li></ul>
  </div>
  <div>
    <h3>OWASP ZAP Full Scan</h3>
    <ul><li>ใช้เมื่อรัน Docker stack ครบ</li><li>สร้าง ZAP context เพื่อจำกัด scope</li><li>รัน Traditional Spider, AJAX Spider, Passive Scan และ Active Scan</li><li>ดึง ZAP alerts มาจัดรูปแบบและ deduplicate</li></ul>
  </div>
</div>

---
class: px-14 py-10
---

## AI และการป้องกันข้อมูลหลุด

<p class="opacity-70">AI ใช้เพื่ออธิบายผล ไม่ใช่เพื่อส่งข้อมูลดิบออกนอกระบบ</p>

<div class="grid grid-cols-3 gap-5 mt-8">
  <div class="border rounded p-5"><h3>ข้อมูลที่ส่งเข้า AI</h3><ul><li>ชื่อช่องโหว่</li><li>ระดับความเสี่ยง</li><li>CWE ID ถ้ามี</li><li>description</li><li>solution</li></ul></div>
  <div class="border rounded p-5"><h3>Privacy Guard</h3><ul><li>redact api_key/token/secret</li><li>redact Authorization/Cookie</li><li>redact private key/AWS key/email</li><li>ตัด query string เป็น [REDACTED_QUERY]</li></ul></div>
  <div class="border rounded p-5"><h3>Local LLM</h3><ul><li>AI_PROVIDER=ollama</li><li>ALLOW_EXTERNAL_AI=false</li><li>OLLAMA_HOST=localhost</li><li>Model: qwen2.5:7b</li></ul></div>
</div>

---
class: px-14 py-10
---

## การประเมินผล

<p class="opacity-70">ใช้หลักฐาน 3 แบบเพื่อยืนยันว่าระบบทำงานได้จริง</p>

<div class="grid grid-cols-5 gap-4 mt-8 text-center">
  <div class="border rounded p-4"><div class="text-4xl font-bold">5</div><p>Real Findings</p></div>
  <div class="border rounded p-4"><div class="text-4xl font-bold">1</div><p>Medium</p></div>
  <div class="border rounded p-4"><div class="text-4xl font-bold">3</div><p>Low</p></div>
  <div class="border rounded p-4"><div class="text-4xl font-bold">12</div><p>Tests OK</p></div>
  <div class="border rounded p-4"><div class="text-4xl font-bold">Local</div><p>AI</p></div>
</div>

<div class="grid grid-cols-3 gap-5 mt-8">
  <div><h3>API Evidence</h3><p><code>scan-result.json</code> จาก <code>/api/scan</code> และ <code>/api/status</code> แสดง alert, summary, OWASP coverage และ engine ที่ใช้</p></div>
  <div><h3>Visual Evidence</h3><p>screenshot หน้า UI, module selector, dashboard, finding detail และ AI explanation จากระบบจริง</p></div>
  <div><h3>Test Evidence</h3><p>unit tests ครอบคลุม baseline scan, OWASP mapping และ AI privacy guard</p></div>
</div>

---
layout: center
class: text-center
---

# ส่วนที่ 3

## ซอฟต์แวร์และอุปกรณ์ที่ใช้

เทคโนโลยีที่ใช้ในการสร้างและพัฒนาชิ้นงาน

---
class: px-14 py-10
---

# ซอฟต์แวร์และอุปกรณ์

## Technology Stack

<p class="opacity-70">แบ่งเทคโนโลยีตามหน้าที่ของระบบ</p>

<div class="grid grid-cols-4 gap-5 mt-8">
  <div><h3>Frontend</h3><ul><li>HTML / CSS / JavaScript</li><li>Bootstrap 5.3.3</li><li>Bootstrap Icons</li><li>marked.js</li><li>localStorage history</li></ul></div>
  <div><h3>Backend</h3><ul><li>Python 3.14.5</li><li>FastAPI</li><li>Uvicorn</li><li>Pydantic v2</li><li>requests</li></ul></div>
  <div><h3>Scanner</h3><ul><li>OWASP ZAP</li><li>Celery</li><li>Redis</li><li>python-owasp-zap</li><li>baseline scanner</li></ul></div>
  <div><h3>AI</h3><ul><li>Ollama</li><li>qwen2.5:7b</li><li>local API</li><li>Thai prompt</li><li>privacy guard</li></ul></div>
</div>

---
class: px-14 py-10
---

## API และ Infrastructure

<p class="opacity-70">FastAPI เป็นแกนกลาง ส่วน Docker stack ใช้สำหรับ full scan</p>

<div class="grid grid-cols-3 gap-6 mt-8">
  <div><h3>FastAPI Endpoints</h3><ul><li><code>GET /</code></li><li><code>POST /api/scan</code></li><li><code>GET /api/status/{task_id}</code></li><li><code>POST /api/explain</code></li></ul></div>
  <div><h3>Docker Services</h3><ul><li>redis: message broker</li><li>zap: OWASP ZAP daemon</li><li>api: FastAPI backend</li><li>worker: Celery scan worker</li></ul></div>
  <div><h3>Local Environment</h3><ul><li>127.0.0.1:8000</li><li>localhost:11434</li><li>Ollama qwen2.5:7b</li><li>Chrome headless screenshots</li></ul></div>
</div>

---
layout: center
class: text-center
---

# ส่วนที่ 4

## ความคืบหน้า

สรุปความคืบหน้าทั้งหมดนับจากการนำเสนอครั้งล่าสุด

---
class: px-14 py-10
---

## สถานะล่าสุดของโครงงาน

<p class="opacity-70">จาก prototype ไปสู่ระบบที่ตรวจจริงและมีหลักฐานประกอบ</p>

<div class="grid grid-cols-6 gap-3 mt-8 text-center">
  <div class="border rounded p-4"><div class="text-xl font-bold text-emerald-600">Done</div><p>Web UI</p></div>
  <div class="border rounded p-4"><div class="text-xl font-bold text-emerald-600">Done</div><p>API</p></div>
  <div class="border rounded p-4"><div class="text-xl font-bold text-emerald-600">Done</div><p>Scanner</p></div>
  <div class="border rounded p-4"><div class="text-xl font-bold text-emerald-600">Done</div><p>AI Local</p></div>
  <div class="border rounded p-4"><div class="text-3xl font-bold">12</div><p>Tests</p></div>
  <div class="border rounded p-4"><div class="text-3xl font-bold">5</div><p>Findings</p></div>
</div>

<div class="grid grid-cols-2 gap-8 mt-8">
  <div><h3>สิ่งที่แก้ไขและพัฒนาเพิ่ม</h3><ul><li>เพิ่ม baseline scanner เพื่อให้ตรวจได้ทันที</li><li>เพิ่ม OWASP coverage และ scan config ในรายงาน</li><li>ปรับ Ollama ให้เริ่มจาก localhost/127.0.0.1</li><li>เพิ่ม privacy tests สำหรับ AI</li></ul></div>
  <div><h3>สิ่งที่ยืนยันแล้ว</h3><ul><li>สแกน target จริงบน localhost สำเร็จ</li><li>AI explanation ทำงานผ่าน Ollama local</li><li>unit tests ผ่านครบ 12 เคส</li></ul></div>
</div>

---
class: px-14 py-10
---

## หลักฐานผลสแกนจริง

<p class="opacity-70">Target ที่ใช้ทดสอบ: <code>http://127.0.0.1:8000/</code></p>

<div class="grid grid-cols-[2fr_1fr] gap-6 mt-6 items-start">
  <div class="rounded border overflow-hidden bg-white">
  <img src="./images/image-20-1.png" alt="Webpentest system screenshot" style="width:100%; display:block;" />

  </div>
  <div class="border-l-4 border-rose-500 pl-5">
    <h3>สรุปผล</h3>
    <ul><li>Engine: baseline</li><li>Selected: A05, A07</li><li>Findings: 5</li><li>Medium: 1</li><li>Low: 3</li><li>Info: 1</li><li>URLs found: 2</li></ul>
  </div>
</div>

---
class: px-14 py-10
---

## หลักฐาน Unit Test

<p class="opacity-70">ทดสอบส่วนสำคัญของระบบเพื่อยืนยัน logic</p>

<div class="grid grid-cols-3 gap-5 mt-8">
  <div><h3>Baseline Scan</h3><ul><li>พบ Missing CSP</li><li>พบ Cookie Without HttpOnly</li><li>พบ exposed .env</li><li>รองรับ 404 โดยไม่ crash</li></ul></div>
  <div><h3>OWASP Mapping</h3><ul><li>normalize current/legacy IDs</li><li>reject invalid IDs</li><li>map ZAP tags</li><li>map CWE/keywords</li></ul></div>
  <div><h3>AI Privacy</h3><ul><li>redact secrets</li><li>redact query string</li><li>block external AI</li><li>prefer localhost Ollama</li></ul></div>
</div>

<div class="mt-8 text-2xl font-bold text-emerald-600">ผลล่าสุด: Ran 12 tests in 0.611s - OK</div>

---
layout: center
class: text-center
---

# ส่วนที่ 5

## ชิ้นงาน

นำเสนอชิ้นงานที่สมบูรณ์แล้ว

---
class: px-14 py-10
---

## หน้าจอหลักและการเลือก Module

<p class="opacity-70">ผู้ใช้สามารถกรอก URL แล้วเลือก Scan All หรือ Scan Selected ได้</p>

<div class="grid grid-cols-[2fr_1fr] gap-6 mt-6 items-start">
  <div class="rounded border overflow-hidden bg-white">
    <img src="./images/image-23-1.png" alt="Webpentest system screenshot" style="width:100%; display:block;" />
  </div>
  <div class="border-l-4 border-blue-500 pl-5">
    <h3>ความสามารถ</h3>
    <ul><li>กรอก Target URL</li><li>เลือก OWASP A01-A10</li><li>Scan All หรือเฉพาะ module</li><li>แสดงจำนวน module ที่เลือก</li><li>ประเมินเวลาสแกน</li></ul>
  </div>
</div>

---
class: px-14 py-10
---

## Dashboard รายงานผล

<p class="opacity-70">รายงานผลรวมช่วยให้เห็นความเสี่ยงและ coverage ได้เร็ว</p>

<div class="grid grid-cols-[2fr_1fr] gap-6 mt-6 items-start">
  <div class="rounded border overflow-hidden bg-white">
    <img src="./images/image-24-1.png" alt="Webpentest system screenshot" style="width:100%; display:block;" />
  </div>
  <div class="border-l-4 border-emerald-500 pl-5">
    <h3>อ่านผลได้ทันที</h3>
    <ul><li>สถานะสแกน</li><li>High / Medium / Low / Info</li><li>จำนวน URL ที่พบ</li><li>จำนวนช่องโหว่รวม</li><li>OWASP coverage</li><li>engine scope</li></ul>
  </div>
</div>

---
class: px-14 py-10
---

## รายละเอียดช่องโหว่

<p class="opacity-70">ตัวอย่าง finding: Missing Content Security Policy</p>

<div class="grid grid-cols-[2fr_1fr] gap-6 mt-6 items-start">
  <div class="rounded border overflow-hidden bg-white">
    <img src="./images/image-25-1.png" alt="Webpentest system screenshot" style="width:100%; display:block;" />
  </div>
  <div class="border-l-4 border-rose-500 pl-5">
    <h3>ข้อมูลที่แสดง</h3>
    <ul><li>Risk: Medium</li><li>Method: GET</li><li>URL</li><li>Evidence</li><li>Description</li><li>Solution</li><li>OWASP A05</li></ul>
  </div>
</div>

---
class: px-14 py-10
---

## AI Explanation

<p class="opacity-70">Ollama local ช่วยอธิบายผลให้ผู้พัฒนาเข้าใจและแก้ไขต่อได้</p>

<div class="grid grid-cols-[2fr_1fr] gap-6 mt-6 items-start">
  <div class="rounded border overflow-hidden bg-white">
    <img src="./images/image-26-1.png" alt="Webpentest system screenshot" style="width:100%; display:block;" />
  </div>
  <div class="border-l-4 border-violet-500 pl-5">
    <h3>โครงสร้างคำตอบ</h3>
    <ul><li>Impact</li><li>Scenario</li><li>Remediation</li><li>Verification</li><li>ภาษาไทย</li><li>Markdown</li></ul>
  </div>
</div>

---
class: px-14 py-10
---

## แนวทางสาธิตหน้าห้อง

<p class="opacity-70">ลำดับ demo ที่ปลอดภัยและควบคุมเวลาได้</p>

<div class="grid grid-cols-7 gap-3 mt-8 text-sm">
  <div class="border rounded p-3"><div class="text-xl font-bold">1</div><h3>เปิดระบบ</h3><p>เข้า <code>http://127.0.0.1:8000/</code></p></div>
  <div class="border rounded p-3"><div class="text-xl font-bold">2</div><h3>กรอก Target</h3><p>ใช้ local lab หรือเว็บที่ได้รับอนุญาต</p></div>
  <div class="border rounded p-3"><div class="text-xl font-bold">3</div><h3>เลือก Module</h3><p>เช่น A05/A07 เพื่อ demo เร็ว</p></div>
  <div class="border rounded p-3"><div class="text-xl font-bold">4</div><h3>เริ่มสแกน</h3><p>อธิบาย engine และ progress</p></div>
  <div class="border rounded p-3"><div class="text-xl font-bold">5</div><h3>อ่านรายงาน</h3><p>ชี้ summary และ OWASP coverage</p></div>
  <div class="border rounded p-3"><div class="text-xl font-bold">6</div><h3>เปิด Finding</h3><p>ชี้ evidence และ solution</p></div>
  <div class="border rounded p-3"><div class="text-xl font-bold">7</div><h3>ถาม AI</h3><p>ให้ Ollama อธิบายเป็นภาษาไทย</p></div>
</div>

---
class: px-14 py-10
---

## ข้อจำกัดและแนวทางพัฒนาต่อ

<p class="opacity-70">ระบุขอบเขตของระบบอย่างตรงไปตรงมา พร้อมแนวทางต่อยอด</p>

<div class="grid grid-cols-3 gap-5 mt-8">
  <div><h3>ข้อจำกัด Scanner</h3><ul><li>baseline ตรวจเฉพาะพื้นฐาน</li><li>business logic ต้อง manual</li><li>authenticated scan ยังต้องต่อยอด</li><li>false positive ต้องยืนยัน</li></ul></div>
  <div><h3>ข้อจำกัด AI</h3><ul><li>AI อาจอธิบายเกินบริบท</li><li>ต้องใช้ผู้เชี่ยวชาญตรวจซ้ำ</li><li>local model ใช้ทรัพยากรเครื่อง</li><li>ควรมี evaluation set</li></ul></div>
  <div><h3>แนวทางต่อยอด</h3><ul><li>authenticated scanning</li><li>export PDF/HTML report</li><li>dependency scanning</li><li>auth/RBAC/rate limit</li><li>database report history</li></ul></div>
</div>

---
class: px-14 py-10
---

# สรุป

## สรุปผลโครงงาน

<div class="mt-6 text-xl">
Wabpentest เป็นระบบตรวจช่องโหว่เว็บที่ใช้งานได้จริง มี AI local และมีหลักฐานประกอบ
</div>

<div class="grid grid-cols-3 gap-5 mt-8">
  <div><h3>สิ่งที่ทำสำเร็จ</h3><ul><li>UI + API พร้อมใช้งาน</li><li>scanner pipeline ทำงานจริง</li><li>OWASP mapping ชัดเจน</li><li>AI explanation ผ่าน Ollama</li></ul></div>
  <div><h3>หลักฐาน</h3><ul><li>screenshot จากระบบจริง</li><li>scan-result.json</li><li>unit tests 12 OK</li><li>PDF render ตรวจแล้ว</li></ul></div>
  <div><h3>ประโยชน์</h3><ul><li>ช่วยเรียนรู้ OWASP Top 10</li><li>ช่วยอ่านผล scanner</li><li>ลดเวลาทำ remediation note</li><li>ลดการส่งข้อมูลออกนอกเครื่อง</li></ul></div>
</div>

<div class="mt-10 text-3xl font-bold">Q&A</div>
