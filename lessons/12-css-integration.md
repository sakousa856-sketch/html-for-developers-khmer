# មេរៀនទី ១២៖ ការភ្ជាប់ CSS ជាមួយ HTML (HTML CSS Integration)

> **CSS (Cascading Style Sheets) ត្រូវបានប្រើដើម្បីរចនារូបរាង ប្លង់ និងពណ៌នៃគេហទំព័រ HTML។**

---

## ១. វិធីទាំង ៣ ក្នុងការបញ្ចូល CSS ទៅក្នុង HTML (3 Ways to Add CSS)

យើងអាចភ្ជាប់ CSS ជាមួយ HTML តាម ៣ របៀប៖

1. **Inline CSS:** សរសេរនៅក្នុង `style` attribute ផ្ទាល់លើ HTML Element
2. **Internal CSS:** សរសេរនៅក្នុង Tag `<style>` ខាងក្នុងផ្នែក `<head>`
3. **External CSS:** សរសេរក្នុង File `.css` ដាច់ដោយឡែក ហើយភ្ជាប់តាមរយៈ Tag `<link>`

---

## ២. ការពន្យល់ និងឧទាហរណ៍ជាក់ស្តែង

### ១. Inline CSS (សរសេរផ្ទាល់លើ Element)
* ប្រើសម្រាប់តែ Element ជាក់លាក់មួយប៉ុណ្ណោះ៖
```html
<h1 style="color: blue; text-align: center;">ចំណងជើង Inline CSS</h1>
```

### ២. Internal CSS (សរសេរក្នុង `<head>`)
* ប្រើសម្រាប់ទំព័រ HTML តែមួយទំព័រ៖
```html
<!DOCTYPE html>
<html>
<head>
  <style>
    body {
      background-color: #f1f5f9;
      font-family: sans-serif;
    }
    h1 {
      color: #0284c7;
    }
    p {
      color: #334155;
      font-size: 16px;
    }
  </style>
</head>
<body>
  <h1>Internal CSS Example</h1>
  <p>ស្ទីលទាំងអស់នៅក្នុងទំព័រនេះត្រូវបានកំណត់ក្នុង Tag style។</p>
</body>
</html>
```

### ៣. External CSS (ភ្ជាប់ File ខាងក្រៅ - ណែនាំខ្លាំងបំផុត ⭐⭐⭐)
* ជាស្តង់ដារវិជ្ជាជីវៈ (Best Practice) ដោយសារវាបំបែក Structure (HTML) និង Style (CSS) ដាច់ពីគ្នា និងអាចចែករំលែកប្រើប្រាស់លើទំព័ររាប់រយបាន៖

**File `index.html`:**
```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1 class="main-title">External CSS</h1>
</body>
</html>
```

**File `style.css`:**
```css
body {
  margin: 0;
  padding: 20px;
  background-color: #ffffff;
}

.main-title {
  color: #16a34a;
  font-size: 28px;
}
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. តើវិធីទាំង ៣ នៃការបញ្ចូល CSS មួយណាជាជម្រើសល្អបំផុតសម្រាប់គេហទំព័រធំៗ? ហេតុអ្វី?
2. ចូរបង្កើត file `index.html` និង file `style.css` រួចភ្ជាប់វាជាមួយ Tag `<link>` ដើម្បីរចនាទំព័រមួយឱ្យមានផ្ទៃខាងក្រោយពណ៌ស្រស់ស្អាត។
