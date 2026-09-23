# មេរៀនទី ១៥៖ Favicon និងចំណងជើង Tab (HTML Favicon & Page Title)

> **Favicon គឺជារូបភាពតូច (Icon) ដែលបង្ហាញនៅលើ Browser Tab នៅក្បែរ Page Title ជួយឱ្យអ្នកប្រើប្រាស់ងាយស្រួលចំណាំគេហទំព័រ។**

---

## ១. ការកំណត់ Page Title (`<title>`)

Tag `<title>` ត្រូវតែស្ថិតនៅក្នុងផ្នែក `<head>` ជានិច្ច៖
* កំណត់ចំណងជើងទំព័រលើ Browser Tab
* កំណត់ឈ្មោះពេលអ្នកប្រើប្រាស់ចុច Bookmark / Favorite
* បង្ហាញជាចំណងជើងធំនៅលើទំព័រស្វែងរករបស់ **Google Search Results (SEO)**

```html
<head>
  <title>វគ្គសិក្សា HTML5 ស្តង់ដារពេញលេញ</title>
</head>
```

---

## ២. របៀបដាក់ Favicon លើគេហទំព័រ (Adding a Favicon)

ដើម្បីដាក់ Favicon យើងត្រូវប្រើប្រាស់ Tag `<link>` នៅក្នុងផ្នែក `<head>`៖

```html
<!DOCTYPE html>
<html lang="km">
<head>
  <meta charset="UTF-8">
  <title>គេហទំព័ររបស់ខ្ញុំ</title>
  
  <!-- ដាក់ Favicon (ទ្រង់ទ្រាយ .ico, .png ឬ .svg) -->
  <link rel="icon" type="image/x-icon" href="favicon.ico">
  
  <!-- ឬប្រើប្រាស់រូបភាព PNG -->
  <!-- <link rel="icon" type="image/png" href="favicon.png"> -->
</head>
<body>
  <h1>ទំព័រនេះមាន Favicon លើ Browser Tab!</h1>
</body>
</html>
```

---

## ៣. ទំហំ និងប្រភេទ File ដែលគាំទ្រសម្រាប់ Favicon

| File Format | ប្រភេទ MIME Type | ទំហំសមស្រប (Sizes) |
| :--- | :--- | :--- |
| **`.ico`** | `image/x-icon` | 16x16, 32x32, 48x48 (គាំទ្រគ្រប់ Browser ចាស់និងថ្មី) |
| **`.png`** | `image/png` | 32x32, 192x192 |
| **`.svg`** | `image/svg+xml` | Scalable (គាំទ្រ Dark Mode លើ Browser ទំនើប) |

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរពន្យល់ពីតួនាទីរបស់ `<title>` ក្នុងការជួយដល់ SEO។
2. បង្កើតឯកសារ HTML មួយ រួចដាក់រូប Favicon `.png` ឬ `.ico` ឱ្យបង្ហាញនៅលើ Browser Tab របស់អ្នក។
