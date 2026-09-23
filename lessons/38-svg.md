# មេរៀនទី ៣៨៖ រូបភាពវ៉ិចទ័រ (HTML5 SVG)

> **SVG (Scalable Vector Graphics) គឺជាភាសា XML សម្រាប់ពិពណ៌នាក្រាហ្វិកពីរវិមាត្រ (2D Graphics) ដែលអាចពង្រីកទំហំដោយមិនបែកព្រាលឡើយ។**

---

## ១. ការប្រើប្រាស់ Tag `<svg>` ក្នុង HTML5

យើងអាចសរសេរកូដ SVG ដោយផ្ទាល់នៅក្នុងឯកសារ HTML៖

```html
<svg width="300" height="200" style="border: 1px solid #e2e8f0;">
  <!-- រាងចតុកោណ (Rectangle) -->
  <rect x="20" y="20" width="100" height="80" fill="#3b82f6" rx="8" />

  <!-- រាងរង្វង់ (Circle) -->
  <circle cx="180" cy="60" r="40" fill="#10b981" stroke="#047857" stroke-width="3" />

  <!-- បន្ទាត់ (Line) -->
  <line x1="20" y1="140" x2="280" y2="140" stroke="#ef4444" stroke-width="4" />

  <!-- អត្ថបទ (Text) -->
  <text x="20" y="180" font-family="sans-serif" font-size="16" fill="#1e293b">Hello SVG Graphic!</text>
</svg>
```

---

## ២. តារាងប្រៀបធៀបរវាង Canvas vs SVG

| លក្ខណៈសម្បត្តិ | HTML5 Canvas | HTML5 SVG |
| :--- | :--- | :--- |
| **មូលដ្ឋានបច្ចេកវិទ្យា** | Pixel-based (Raster) | Vector-based (XML) |
| **ភាសាបញ្ជា** | បញ្ជាតាម **JavaScript** សុទ្ធ | បញ្ជាតាម **HTML/XML Tags + CSS** |
| **គុណភាពពេល Zoom** | បែក Pixel ពេលពង្រីកធំ | **មិនបែកព្រាលឡើយ (Crystal Clear)** |
| **ការភ្ជាប់ Event (DOM)** | គ្មាន Event លើរូបភាពនីមួយៗទេ | អាចចាប់ Event (`onclick`, `hover`) លើ Element នីមួយៗបាន |
| **ការប្រើប្រាស់ល្អបំផុត** | Web Games, Video Processing, Pixels | **Icons, Logos, UI Illustrations, UI Charts** |

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរពន្យល់ពីមូលហេតុដែលគេនិយមប្រើ SVG សម្រាប់ Logo និង Icons នៃគេហទំព័រទំនើប។
2. បង្កើតរូបតំណាងផ្កាយ ឬរាងធរណីមាត្រចម្រុះពណ៌ដោយប្រើ `<svg>`, `<polygon>`, និង `<circle>`។
