# មេរៀនទី ២៤៖ ផ្នែកក្បាលគេហទំព័រ និង Meta Tags (HTML Head & Meta Elements)

> **ផ្នែក `<head>` គឺជាកន្លែងផ្ទុកទិន្នន័យសម្គាល់ (Metadata) អំពីទំព័រ HTML ដែលផ្តល់ព័ត៌មានដល់ Browser និង Search Engines។**

---

## ១. បណ្តា Elements ដែលអាចស្ថិតនៅក្នុង `<head>`

* `<title>`: កំណត់ចំណងជើងទំព័រ
* `<style>`: សរសេរ Internal CSS
* `<link>`: ភ្ជាប់ External Resources (CSS, Favicon, Web Fonts)
* `<meta>`: កំណត់ទិន្នន័យ Metadata (Charset, Viewport, Keywords, Author, SEO)
* `<script>`: បញ្ចូលកូដ JavaScript
* `<base>`: កំណត់ Base URL លំនាំដើមសម្រាប់ Links ទាំងអស់ក្នុងទំព័រ

---

## ២. Meta Tags សំខាន់ៗបំផុតដែលត្រូវតែមាន (Essential Meta Tags)

```html
<head>
  <!-- ១. កំណត់ Character Encoding ជា UTF-8 (ចាំបាច់សម្រាប់ភាសាខ្មែរ) -->
  <meta charset="UTF-8">

  <!-- ២. កំណត់ Viewport សម្រាប់ Responsive Design លើទូរស័ព្ទដៃ -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <!-- ៣. ការពិពណ៌នាសម្រាប់ Search Engine (Google SEO Description) -->
  <meta name="description" content="វគ្គសិក្សា HTML5 ស្តង់ដារពេញលេញជាភាសាខ្មែរ រៀនពីកម្រិតដំបូងដល់កម្រិតខ្ពស់។">

  <!-- ៤. ពាក្យគន្លឹះស្វែងរក (Keywords) -->
  <meta name="keywords" content="HTML, CSS, Web Development, រៀនសរសេរកូដ, ភាសាខ្មែរ">

  <!-- ៥. ឈ្មោះអ្នកនិពន្ធ/ម្ចាស់កម្មសិទ្ធិ -->
  <meta name="author" content="លោកគ្រូ សុខ សាន្ត">

  <!-- ៦. Open Graph Meta Tags (សម្រាប់ Share លើ Facebook / Telegram ឱ្យចេញរូប និងចំណងជើងស្អាត) -->
  <meta property="og:title" content="រៀន HTML5 ជាភាសាខ្មែរ">
  <meta property="og:description" content="មេរៀន Web Development ដកស្រង់ពី W3Schools">
  <meta property="og:image" content="https://example.com/cover.jpg">

  <title>វគ្គសិក្សា HTML5</title>
</head>
```

---

## ៣. Tag `<base>` (Base URL)
Tag `<base>` កំណត់ URL មូលដ្ឋានសម្រាប់រាល់ Relative Links ទាំងអស់ក្នុងទំព័រ៖
```html
<head>
  <base href="https://www.w3schools.com/images/" target="_blank">
</head>
<body>
  <!-- វានឹងក្លាយជា https://www.w3schools.com/images/w3html.gif ស្វ័យប្រវត្តិ -->
  <img src="w3html.gif">
</body>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរបង្កើតផ្នែក `<head>` ពេញលេញមួយដែលមាន `charset`, `viewport`, `description`, `author`, និង `title` ត្រឹមត្រូវតាមស្តង់ដារ SEO។
2. តើហេតុអ្វីបានជា Open Graph Tags (`og:title`, `og:image`) មានសារៈសំខាន់នៅពេល Share Link លើបណ្តាញសង្គម?
