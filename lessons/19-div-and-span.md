# មេរៀនទី ១៩៖ ធាតុ Container `<div>` និង `<span>` (HTML Div & Span)

> **`<div>` និង `<span>` គឺជាធាតុ Non-semantic Containers ដ៏ពេញនិយមបំផុតសម្រាប់ប្រមូលផ្តុំ និងរៀបចំរចនា Style ឬដំណើរការជាមួយ JavaScript។**

---

## ១. ធាតុ `<div>` (Block Container)

`<div>` តំណាងឱ្យ **Division** ឬ **Section**៖
* ជា **Block-level Element**
* គ្មានអត្ថន័យពិសេសលើមាតិកាទេ (Non-semantic)
* ប្រើប្រាស់ជា **Container** សម្រាប់ប្រមូលផ្តុំ Elements ជាច្រើនចូលគ្នា ដើម្បីងាយស្រួលរៀបចំ Layout (CSS Flexbox/Grid) ឬកំណត់ CSS Class រួមមួយ។

```html
<div class="card" style="background: white; border: 1px solid #ccc; padding: 16px; border-radius: 8px;">
  <h2>ចំណងជើងកាត</h2>
  <p>នេះជាការពិពណ៌នានៅក្នុង Div Container។</p>
  <button>ចុចមើលលម្អិត</button>
</div>
```

---

## ២. ធាតុ `<span>` (Inline Container)

`<span>` គឺជា **Inline Container**៖
* មិនចុះបន្ទាត់ថ្មីទេ
* ប្រើសម្រាប់ក្តោបពាក្យ ឬឃ្លាតូចមួយនៅក្នុងកថាខណ្ឌ ដើម្បីកំណត់ Style ជាក់លាក់ (ដូចជា ប្តូរពណ៌អក្សរ ដាក់ Background) ឬបញ្ជាដោយ JavaScript។

```html
<p>
  សួស្តី! ខ្ញុំឈ្មោះ <span style="color: #0284c7; font-weight: bold;">សុខ សាន្ត</span> ហើយខ្ញុំរស់នៅរាជធានី <span style="color: #16a34a;">ភ្នំពេញ</span>។
</p>
```

---

## ៣. ភាពខុសគ្នាសំខាន់រវាង `<div>` និង `<span>`

```text
+-------------------------------------------------------+
|  <div> (Block Container)                              |
|  ពង្រីកពេញទទឹង និងអាចផ្ទុកធាតុផ្សេងៗបានច្រើន         |
+-------------------------------------------------------+

អត្ថបទធម្មតា [ <span>Inline</span> ] អត្ថបទបន្តក្នុងជួរដដែល
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. តើនៅពេលណាដែលយើងគួរប្រើ `<div>` ហើយពេលណាគួរប្រើ `<span>`?
2. ចូរបង្កើត Product Card មួយដោយប្រើ `<div>` ដែលមានរូបភាព ឈ្មោះផលិតផល តម្លៃ និងប៊ូតុង "ទិញឥឡូវនេះ" ដោយប្រើ `<span>` សម្រាប់កំណត់ពណ៌ក្រហមលើតម្លៃទំនិញ។
