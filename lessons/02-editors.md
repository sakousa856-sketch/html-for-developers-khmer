# មេរៀនទី ០២៖ កម្មវិធីសរសេរកូដ HTML (HTML Editors)

> **យើងអាចសរសេរកូដ HTML ដោយប្រើប្រាស់ Text Editor ណាមួយក៏បាន ប៉ុន្តែការប្រើប្រាស់ Professional Code Editor ជួយឱ្យយើងសរសេរកូដបានលឿន ស្អាត និងគ្មាន Error។**

---

## ១. កម្មវិធីសរសេរកូដដែលពេញនិយមបំផុត (Popular HTML Editors)

សម្រាប់ការរៀន និងធ្វើការងារជា Web Developer អាជីព កម្មវិធីដែលត្រូវបានណែនាំឱ្យប្រើរួមមាន៖

1. **Visual Studio Code (VS Code):** (ណែនាំខ្លាំងបំផុត ⭐⭐⭐⭐⭐)
   * ឥតគិតថ្លៃ (Free & Open Source) បង្កើតដោយ Microsoft
   * មាន Extensions រាប់ពាន់ជួយសម្រួលការសរសេរកូដ
   * មាន Built-in Terminal និង Git Integration
2. **Sublime Text:** ស្រាល ដំណើរការលឿន
3. **Notepad++ (Windows) / TextEdit (macOS):** កម្មវិធីធម្មតាសម្រាប់សរសេរបឋម

---

## ២. ជំហានទាំង ៤ ក្នុងការបង្កើតគេហទំព័រដំបូងជាមួយ VS Code (4 Steps)

### ជំហានទី ១: បង្កើត Folder សម្រាប់ Project
* បង្កើត Folder ថ្មីមួយនៅលើកុំព្យូទ័រ (ឧទាហរណ៍ `my-first-website`)
* បើកកម្មវិធី VS Code រួចចូល Menu **File > Open Folder...** ហើយជ្រើសរើស Folder នោះ។

### ជំហានទី ២: បង្កើត File HTML
* ចុចប៊ូតុង **New File** ក្នុង VS Code
* ដាក់ឈ្មោះ file ថា `index.html` (កន្ទុយ `.html` គឺចាំបាច់បំផុត)

> 💡 **ចំណាំ:** ឈ្មោះ `index.html` គឺជាឈ្មោះស្តង់ដារលំនាំដើម (Default Home Page) ដែល Web Server ស្វែងរកដំបូងគេបង្អស់។

### ជំហានទី ៣: សរសេរកូដ HTML
វាយបញ្ចូលកូដខាងក្រោម ឬវាយសញ្ញាឧទាន `!` រួចចុច **Tab / Enter** ដើម្បីឱ្យ VS Code បង្កើត Emmet Boilerplate ស្វ័យប្រវត្តិ៖

```html
<!DOCTYPE html>
<html lang="km">
<head>
  <meta charset="UTF-8">
  <title>គេហទំព័រដំបូងរបស់ខ្ញុំ</title>
</head>
<body>
  <h1>សួស្តីពិភពលោក! (Hello World)</h1>
  <p>ខ្ញុំកំពុងរៀន HTML5 ជាមួយ VS Code។</p>
</body>
</html>
```

### ជំហានទី ៤: បើកមើលលទ្ធផលលើ Browser
* **វិធីទី ១:** Double-click លើ file `index.html` ក្នុង Computer File Explorer ដើម្បីបើកជាមួយ Browser។
* **វិធីទី ២ (ណែនាំ):** ដំឡើង Extension **"Live Server"** ក្នុង VS Code រួច Right-click លើ `index.html` ហើយជ្រើសរើស **"Open with Live Server"**។ រាល់ពេលចុច Save (`Ctrl + S` ឬ `Cmd + S`) Browser នឹង Refresh បង្ហាញលទ្ធផលថ្មីភ្លាមៗ!

---

## ៣. Extension សំខាន់ៗសម្រាប់ VS Code (Recommended Extensions)

* **Live Server (by Ritwick Dey):** បើក Local Development Server ជាមួយ Live Reload
* **Prettier - Code Formatter:** រៀបចំកូដឱ្យមានគម្លាត Tab ស្អាត និងមានរបៀប
* **Auto Rename Tag:** ប្តូរឈ្មោះ Closing Tag ដោយស្វ័យប្រវត្តិតាម Opening Tag

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ដំឡើងកម្មវិធី VS Code និង Extension **Live Server** លើកុំព្យូទ័ររបស់អ្នក។
2. បង្កើត Folder ឈ្មោះ `html-lab-01` និង File `index.html`។
3. សរសេរកូដ HTML បង្ហាញ `<h1>` ដាក់ឈ្មោះសាលា/វិទ្យាស្ថានរបស់អ្នក និង `<p>` ដាក់ព័ត៌មានទំនាក់ទំនង។
4. ដំណើរការវាជាមួយ Live Server។
