# មេរៀនទី ២២៖ ការប្រើ JavaScript ក្នុង HTML (HTML JavaScript Integration)

> **JavaScript ត្រូវបានប្រើដើម្បីបន្ថែមភាពរស់រវើក អន្តរកម្ម (Interactivity) និងការគណនា Logic ទៅលើគេហទំព័រ HTML។**

---

## ១. ការប្រើប្រាស់ Tag `<script>`

Tag `<script>` ត្រូវបានប្រើសម្រាប់សរសេរកូដ JavaScript ដោយផ្ទាល់ ឬភ្ជាប់ទៅកាន់ឯកសារ `.js` ខាងក្រៅ៖

### ១. សរសេរកូដ JS ដោយផ្ទាល់ក្នុង HTML:
```html
<p id="greeting">សូមស្វាគមន៍!</p>
<button onclick="changeText()">ចុចប្តូរអត្ថបទ</button>

<script>
  function changeText() {
    document.getElementById('greeting').innerHTML = '🎉 សួស្តី! អត្ថបទត្រូវបានផ្លាស់ប្តូរដោយ JavaScript!';
    document.getElementById('greeting').style.color = '#16a34a';
  }
</script>
```

### ២. ភ្ជាប់ឯកសារ JS ខាងក្រៅ (External JavaScript):
```html
<!-- ភ្ជាប់ file script.js -->
<script src="main.js"></script>
```

---

## ២. សមត្ថភាពទូទៅរបស់ JavaScript លើ HTML DOM

JavaScript អាច៖
1. **ផ្លាស់ប្តូរមាតិកា HTML (Change Content):** `document.getElementById('demo').innerHTML = 'Hello'`
2. **ផ្លាស់ប្តូរ Style CSS (Change Styles):** `element.style.display = 'none'`
3. **ផ្លាស់ប្តូរ Attribute (Change Attributes):** `document.getElementById('myImg').src = 'pic_on.gif'`
4. **ឆ្លើយតបនឹងព្រឹត្តិការណ៍ (Event Handlers):** `onclick`, `onmouseover`, `oninput`, `onsubmit`

---

## ៣. Tag `<noscript>` (សម្រាប់ Browser ដែលបិទ JavaScript)

ប្រសិនបើអ្នកប្រើប្រាស់បានបិទ (Disable) JavaScript ក្នុង Browser របស់ពួកគេ Tag `<noscript>` នឹងបង្ហាញសារជូនដំណឹង៖

```html
<noscript>
  <p style="color: red;">⚠️ សូមបើក JavaScript ក្នុង Browser របស់អ្នក ដើម្បីដំណើរការគេហទំព័រនេះបានពេញលេញ។</p>
</noscript>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. បង្កើតប៊ូតុងមួយដែលមានសរសេរ `onclick` សម្រាប់បើកប្រអប់ `alert('សួស្តីសិស្សទាំងអស់គ្នា!')`។
2. បង្កើតរូបភាពអំពូលភ្លើងមួយ ដោយមានប៊ូតុង "បើកភ្លើង" (ប្តូរ `src="light_on.png"`) និងប៊ូតុង "បិទភ្លើង" (ប្តូរ `src="light_off.png"`)។
