# មេរៀនទី ៣៩៖ ប្រព័ន្ធផ្សព្វផ្សាយ និង Plugins (HTML Media & Plugins)

> **HTML Multimedia រួមបញ្ចូលទាំង សំឡេង (Audio), តន្ត្រី, រូបភាពមានចលនា, វីដេអូ (Video) និងឯកសារបង្កប់ (Plugins)។**

---

## ១. ទម្រង់ឯកសារប្រព័ន្ធផ្សព្វផ្សាយពេញនិយម (Multimedia Formats)

| ប្រភេទ | Formats ដែលគាំទ្រល្អបំផុតលើ Web | ការពិពណ៌នា |
| :--- | :--- | :--- |
| **Video** | `.mp4`, `.webm`, `.ogg` | **MP4 (H.264)** គាំទ្រគ្រប់ Browser ទាំងអស់ ១០០% |
| **Audio** | `.mp3`, `.wav`, `.ogg`, `.aac` | **MP3** គឺជាស្តង់ដារសំឡេងពេញនិយមបំផុត |

---

## ២. HTML Helper Plug-ins (`<object>` និង `<embed>`)

មុនសម័យ HTML5 កម្មវិធីរុករក Browser ត្រូវការពឹងផ្អែកលើ Plugins ក្រៅ (ដូចជា Adobe Flash Player, Java Applets, QuickTime) ដើម្បីចាក់វីដេអូ ឬសំឡេង។

សព្វថ្ងៃនេះ HTML5 គាំទ្រ Audio និង Video ដោយផ្ទាល់ (Natively) តាមរយៈ `<audio>` និង `<video>` ដោយ **លែងត្រូវការ Flash Player ទៀតហើយ**។

ទោះជាយ៉ាងណា Tag `<object>` និង `<embed>` នៅតែត្រូវបានប្រើសម្រាប់បង្កប់ឯកសារ **PDF** ឬឯកសារ Interactive ខាងក្រៅ៖

```html
<!-- បង្កប់ឯកសារ PDF ក្នុងទំព័រ HTML -->
<object data="document.pdf" type="application/pdf" width="100%" height="500px">
  <p>Browser របស់អ្នកមិនគាំទ្រការបង្ហាញ PDF ទេ។ <a href="document.pdf">ទាញយក PDF ទីនេះ</a></p>
</object>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. តើទ្រង់ទ្រាយវីដេអូមួយណាដែលគាំទ្រលើគ្រប់ Web Browsers ទាំងអស់?
2. សាកល្បងប្រើប្រាស់ Tag `<object>` ដើម្បីបង្កប់ឯកសារ PDF មួយក្នុងទំព័រ HTML របស់អ្នក។
