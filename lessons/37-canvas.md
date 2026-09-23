# មេរៀនទី ៣៧៖ ផ្ទាំងគំនូរកូដ (HTML5 Canvas)

> **HTML5 `<canvas>` គឺជា Element សម្រាប់គូរក្រាហ្វិក (Graphics, Animations, Charts, Games) នៅលើគេហទំព័រ ដោយប្រើប្រាស់ JavaScript។**

---

## ១. ការបង្កើត Canvas Element

Tag `<canvas>` គ្រាន់តែជាផ្ទាំងក្រណាត់ទទេមួយប៉ុណ្ណោះ។ ដើម្បីគូររូបបាន យើងត្រូវប្រើ **JavaScript**៖

```html
<canvas id="myCanvas" width="400" height="200" style="border: 1px solid #cbd5e1;"></canvas>
```

---

## ២. ជំហានក្នុងការគូររូបជាមួយ JavaScript 2D Context

```html
<script>
  // ១. ចាប់យក Canvas Element
  const canvas = document.getElementById('myCanvas');

  // ២. បង្កើត 2D Rendering Context
  const ctx = canvas.getContext('2d');

  // ៣. គូររាងចតុកោណពណ៌ក្រហម (Filled Rectangle)
  ctx.fillStyle = '#ef4444';
  ctx.fillRect(20, 20, 150, 100); // (x, y, width, height)

  // ៤. គូរបន្ទាត់ (Line)
  ctx.beginPath();
  ctx.moveTo(200, 20);
  ctx.lineTo(350, 120);
  ctx.strokeStyle = '#0284c7';
  ctx.lineWidth = 4;
  ctx.stroke();

  // ៥. គូររង្វង់ (Circle / Arc)
  ctx.beginPath();
  ctx.arc(300, 60, 40, 0, 2 * Math.PI); // (x, y, radius, startAngle, endAngle)
  ctx.fillStyle = '#10b981';
  ctx.fill();

  // ៦. សរសេរអក្សរលើ Canvas (Text)
  ctx.font = '20px sans-serif';
  ctx.fillStyle = '#0f172a';
  ctx.fillText('HTML5 Canvas', 20, 160);
</script>
```

---

## ៣. អត្ថប្រយោជន៍ និងការប្រើប្រាស់ជាក់ស្តែងនៃ Canvas

* **Web Games:** គូរចលនាហ្គេម 2D/3D (រួមជាមួយ WebGL)
* **Data Visualization:** បង្កើត Graphs និង Charts (ដូចជា Chart.js, D3.js)
* **Photo Editing / Filters:** កែប្រែពណ៌ និង Pixel នៃរូបភាពលើ Browser

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរបង្កើត Canvas ទំហំ 500x300px រួចគូរទង់ជាតិប្រទេសកម្ពុជា ឬរាងធរណីមាត្រចំនួន ៣ ផ្សេងគ្នា។
2. សាកល្បងសរសេរអត្ថបទឈ្មោះរបស់អ្នកលើ Canvas ដោយប្រើ `ctx.fillText()`។
