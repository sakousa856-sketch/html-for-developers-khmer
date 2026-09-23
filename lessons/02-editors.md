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

## ៣. Extension ពេញនិយមបំផុតសម្រាប់សរសេរ HTML ឱ្យបានលឿន (Top VS Code Extensions)

![Top VS Code Extensions for HTML Development](../assets/vscode-html-extensions.svg)

ដើម្បីបង្កើនល្បឿន និងប្រសិទ្ធភាពក្នុងការសរសេរកូដ Web Development អ្នកគួរដំឡើង Extensions ខាងក្រោមក្នុង VS Code (ចុច `Ctrl + Shift + X` ឬ `Cmd + Shift + X` ដើម្បីស្វែងរកដំឡើង)៖

| # | ឈ្មោះ Extension | អ្នកបង្កើត (Author) | អត្ថប្រយោជន៍ និងមុខងារសំខាន់ៗ |
| :---: | :--- | :--- | :--- |
| **1** | **Live Server** | Ritwick Dey | ⚡ បង្កើត Local Server ជាមួយមុខងារ **Auto-Reload**។ រាល់ពេលចុច Save (`Ctrl+S`) Browser នឹង Refresh បង្ហាញលទ្ធផលភ្លាមៗ ដោយមិនបាច់ចុច Reload ដោយដៃឡើយ។ |
| **2** | **Material Icon Theme** | Philipp Kief | 🎨 ផ្លាស់ប្តូររូប Icon នៃ File និង Folder ឱ្យស្រស់ស្អាត (HTML5, CSS3, JS, Images, Folders) ងាយស្រួលមើលសម្គាល់មិនច្រឡំ។ |
| **3** | **Auto Rename Tag** | Jun Han | 🏷️ ពេលអ្នកកែឈ្មោះ Start Tag (ឧ. `<h1>` ទៅ `<h2>`) នោះ End Tag (`</h1>` ទៅ `</h2>`) នឹងប្តូរតាមដោយស្វ័យប្រវត្តិ មិនបាច់កែពីរដង។ |
| **4** | **Auto Close Tag** | Jun Han | 🔒 ជួយបិទ Closing Tag ដោយស្វ័យប្រវត្ត ពេលអ្នកវាយ `<div` រួចវាយ `>` វានឹងបង្កើត `</div>` ឱ្យភ្លាម។ |
| **5** | **Prettier - Code Formatter** | Prettier | ✨ តម្រឹមកូដ និងគម្លាតបន្ទាត់ (Indentation / Tab) ឱ្យស្អាតមានរបៀបតាមស្តង់ដារ ដោយស្វ័យប្រវត្តពេលចុច Save ឬចុចកាត់ `Shift + Option/Alt + F`។ |
| **6** | **HTML CSS Support** | ecmel | 💡 ជួយ Suggest ឈ្មោះ CSS Class និង ID នៅក្នុង HTML ដោយស្វ័យប្រវត្តិ (IntelliSense)។ |
| **7** | **Highlight Matching Tag** | Vincas Stonys | 🔍 គូសបន្ទាត់សម្គាល់គូ Tag បើក និង Tag បិទ ងាយស្រួលរកកន្លែងកូដវែងៗ។ |
| **8** | **Color Highlight** | Sergii N | 🌈 បង្ហាញពណ៌ពិតប្រាកដលើលេខកូដ HEX, RGB, HSL នៅក្នុង Editor ផ្ទាល់។ |

---

## ⚡ គន្លឹះសរសេរកូដលឿនជាមួយ Emmet (Built-in Shortcuts)

VS Code មានមុខងារ **Emmet** ភ្ជាប់មកស្រាប់៖
* វាយ `!` រួចចុច `Tab` ឬ `Enter` ➔ បង្កើតគ្រោងឆ្អឹង HTML5 ពេញលេញភ្លាមៗ
* វាយ `h1.title` ➔ បង្កើត `<h1 class="title"></h1>`
* វាយ `ul>li*3` ➔ បង្កើត `<ul>` ដែលមាន `<li>` ចំនួន ៣ ខាងក្នុង
* វាយ `p.text#main` ➔ បង្កើត `<p class="text" id="main"></p>`

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Lab 01)

1. ដំឡើងកម្មវិធី VS Code និងបណ្តា Extension ពេញនិយម (**Live Server**, **Material Icon Theme**, **Auto Rename Tag**...)។
2. បង្កើត Folder ឈ្មោះ `html-lab-01` និង File `index.html`។
3. សរសេរកូដ HTML បង្ហាញ `<h1>` ដាក់ឈ្មោះសាលា/វិទ្យាស្ថានរបស់អ្នក និង `<p>` ដាក់ព័ត៌មានទំនាក់ទំនង។
4. ដំណើរការវាជាមួយ **Live Server** (Right-click លើ `index.html` > **Open with Live Server**)។

👉 **កូដគំរូដំណោះស្រាយពេញលេញ:** មើលក្នុង folder [exercises/html-lab-01/index.html](../exercises/html-lab-01/index.html)
