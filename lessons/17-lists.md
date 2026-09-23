# មេរៀនទី ១៧៖ បញ្ជីរាយនាម (HTML Lists)

> **HTML Lists អនុញ្ញាតឱ្យយើងរៀបចំក្រុមនៃព័ត៌មានដែលទាក់ទងគ្នាជាបញ្ជីរាយនាម។**

---

## ១. ប្រភេទទាំង ៣ នៃ HTML Lists

1. **Unordered List (`<ul>`):** បញ្ជីគ្មានលេខរៀង (ប្រើសញ្ញា Dots / Bullets)
2. **Ordered List (`<ol>`):** បញ្ជីមានលេខរៀងលំដាប់លំដោយ (1, 2, 3... ឬ A, B, C...)
3. **Description List (`<dl>`):** បញ្ជីពន្យល់និយមន័យ (Term & Description)

---

## ២. ការពន្យល់ និងឧទាហរណ៍កូដ

### ១. Unordered HTML List (`<ul>` និង `<li>`)
ធាតុនីមួយៗក្នុងបញ្ជីត្រូវបានកំណត់ដោយ Tag `<li>` (List Item)៖
```html
<ul>
  <li>កាហ្វេ (Coffee)</li>
  <li>តែ (Tea)</li>
  <li>ទឹកដោះគោ (Milk)</li>
</ul>
```

### ២. Ordered HTML List (`<ol>` និង `<li>`)
យើងអាចប្រើប្រាស់ attribute `type` ដើម្បីកំណត់ទម្រង់លេខរៀង (`1`, `A`, `a`, `I`, `i`)៖
```html
<!-- លេខរៀងជាអក្សរឡាតាំងធំ A, B, C -->
<ol type="A">
  <li>ដំណាក់កាលទី ១៖ រៀបចំគម្រោង</li>
  <li>ដំណាក់កាលទី ២៖ សរសេរកូដ</li>
  <li>ដំណាក់កាលទី ៣៖ តេស្ត និង Deploy</li>
</ol>
```

### ៣. Nested List (បញ្ជីបង្កប់ក្នុងបញ្ជី)
```html
<ul>
  <li>ភាសា Frontend
    <ul>
      <li>HTML5</li>
      <li>CSS3</li>
      <li>JavaScript</li>
    </ul>
  </li>
  <li>ភាសា Backend
    <ul>
      <li>PHP (Laravel)</li>
      <li>Java (Spring Boot)</li>
    </ul>
  </li>
</ul>
```

### ៤. Description List (`<dl>`, `<dt>`, `<dd>`)
* `<dl>`: Description List
* `<dt>`: Description Term (ពាក្យគន្លឹះ)
* `<dd>`: Description Data (សេចក្តីពន្យល់)
```html
<dl>
  <dt><b>HTML</b></dt>
  <dd>HyperText Markup Language - ភាសាសាងសង់រចនាសម្ព័ន្ធ Web</dd>
  <dt><b>CSS</b></dt>
  <dd>Cascading Style Sheets - ភាសារចនា Style និង Color</dd>
</dl>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរបង្កើតបញ្ជីរាយមុខម្ហូប (Nested List) ដែលមានបែងចែកជា "ម្ហូបពេលព្រឹក", "ម្ហូបពេលថ្ងៃត្រង់", និង "ភេសជ្ជៈ"។
2. បង្កើត Description List `<dl>` មួយដែលពន្យល់ពាក្យបច្ចេកទេសចំនួន ៤ (Frontend, Backend, Database, Server)។
