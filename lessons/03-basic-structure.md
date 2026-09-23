# មេរៀនទី ០៣៖ រចនាសម្ព័ន្ធមូលដ្ឋាននៃឯកសារ HTML (HTML Basic Document Structure)

> **ឯកសារ HTML ទាំងអស់ត្រូវតែមានរចនាសម្ព័ន្ធគ្រោងឆ្អឹងស្តង់ដារមួយ ដើម្បីឱ្យ Browser អាច Render បានត្រឹមត្រូវ។**

---

## ១. គ្រោងឆ្អឹងស្តង់ដារ HTML5 (HTML5 Skeleton)

```html
<!DOCTYPE html>
<html lang="km">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ចំណងជើងគេហទំព័រ</title>
</head>
<body>

  <h1>ចំណងជើងធំ (Heading 1)</h1>
  <p>ខ្លឹមសារអត្ថបទកថាខណ្ឌ (Paragraph Content)</p>

</body>
</html>
```

---

## ២. ការពន្យល់លម្អិតអំពីផ្នែកនីមួយៗ (Detailed Breakdown)

### ១. `<!DOCTYPE html>`
* **Document Type Declaration:** មិនមែនជា HTML Tag ទេ ប៉ុន្តែជាការប្រកាសប្រាប់ Browser ថាឯកសារនេះប្រើប្រាស់ស្តង់ដារ **HTML5**។
* ត្រូវតែស្ថិតនៅ **បន្ទាត់ទី ១ លើគេបង្អស់** ក្នុងឯកសារ ដោយមិន Case-sensitive ឡើយ (អាចសរសេរ `<!doctype html>` ឬ `<!DOCTYPE HTML>`)។

### ២. `<html lang="km">`
* គឺជា **Root Element** របស់ឯកសារ HTML។
* Attribute `lang="km"` កំណត់ភាសារបស់គេហទំព័រ (ភាសាខ្មែរ) ដែលជួយដល់ Search Engines (SEO) និង Screen Readers ក្នុងការបញ្ចេញសំឡេងត្រឹមត្រូវ។

### ៣. `<head>` Element
* ផ្ទុកព័ត៌មានបច្ចេកទេស (Metadata) នៃគេហទំព័រ ដែល **មិនបង្ហាញលើអេក្រង់មាតិកាផ្ទាល់ឡើយ**៖
  * `<meta charset="UTF-8">`: កំណត់ Character Encoding ជា UTF-8 ដើម្បីឱ្យ Browser អាចបង្ហាញអក្សរខ្មែរ (Unicode) និងភាសាដទៃទៀតបានត្រឹមត្រូវ ១០០% ដោយមិនចេញសញ្ញាសួរ (?) ឬអក្សរខូច។
  * `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: បង្កើនភាព Responsive លើទូរស័ព្ទដៃ និង Tablet។
  * `<title>`: ឈ្មោះចំណងជើងដែលបង្ហាញលើ Browser Tab ឬលើលទ្ធផលស្វែងរករបស់ Google។

### ៤. `<body>` Element
* ផ្ទុកមាតិកាដែលអាចមើលឃើញទាំងអស់ (Visible Page Content) ដូចជា អត្ថបទ រូបភាព វីដេអូ តារាង ប៊ូតុង និងទម្រង់បែបបទ។ ក្នុងឯកសារ HTML មួយ មាន `<body>` តែមួយគត់។

---

## ៣. រចនាសម្ព័ន្ធដើមឈើនៃ HTML (HTML DOM Tree Structure)

```text
<html>
  ├── <head>
  │     ├── <meta charset="UTF-8">
  │     ├── <meta name="viewport" ...>
  │     └── <title> ... </title>
  │
  └── <body>
        ├── <h1> ... </h1>
        ├── <p> ... </p>
        └── <div> ... </div>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរពន្យល់ពីសារៈសំខាន់នៃ `<meta charset="UTF-8">` ចំពោះភាសាខ្មែរ។
2. តើអ្វីជាភាពខុសគ្នារវាងផ្នែក `<head>` និងផ្នែក `<body>`?
3. ចូរបង្កើត file `about.html` ដោយសរសេររចនាសម្ព័ន្ធ HTML5 ពេញលេញ រួចដាក់ `<title>` ថា "អំពីខ្ញុំ" និង `<h1>` ថា "ស្វាគមន៍មកកាន់ទំព័រផ្ទាល់ខ្លួន"។
