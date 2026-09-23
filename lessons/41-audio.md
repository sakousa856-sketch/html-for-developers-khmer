# មេរៀនទី ៤១៖ សំឡេងក្នុង HTML (HTML Audio)

> **Tag `<audio>` ក្នុង HTML5 ត្រូវបានប្រើសម្រាប់ចាក់សំឡេង តន្ត្រី ឬ Podcast នៅលើគេហទំព័រ។**

---

## ១. ទម្រង់សរសេរ HTML Audio

```html
<audio controls>
  <source src="podcast.mp3" type="audio/mpeg">
  <source src="podcast.ogg" type="audio/ogg">
  Browser របស់អ្នកមិនគាំទ្រ Audio tag ទេ។
</audio>
```

---

## ២. បណ្តា Attributes សំខាន់ៗរបស់ `<audio>`

| Attribute | ការពន្យល់ (Description) |
| :--- | :--- |
| `controls` | បង្ហាញផ្ទាំងបញ្ជា (ប៊ូតុង Play/Pause, កម្រិតសំឡេង, Timeline) |
| `autoplay` | ចាក់សំឡេងស្វ័យប្រវត្តិពេល load ទំព័រ (Browser ភាគច្រើនរឹតបន្តឹង) |
| `muted` | បិទសំឡេងជាមុន (Mute) |
| `loop` | ចាក់សំឡេងវិលជុំវិញសារឡើងវិញ |
| `preload` | កំណត់ការ Load សំឡេងទុកជាមុន (`auto`, `metadata`, `none`) |

---

## ៣. ទម្រង់សំឡេងដែល Browser គាំទ្រ (Supported Audio Formats)

| Format | MIME-type | ការគាំទ្រ (Browser Support) |
| :--- | :--- | :--- |
| **MP3** | `audio/mpeg` | គាំទ្រគ្រប់ Browser ទាំងអស់ (Chrome, Safari, Edge, Firefox) |
| **WAV** | `audio/wav` | គាំទ្រគ្រប់ Browser ទាំងអស់ (ទំហំធំ គ្មានការបង្រួម) |
| **OGG** | `audio/ogg` | គាំទ្រលើ Chrome, Firefox, Opera |

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរបង្កើត Music Player សាមញ្ញមួយដោយប្រើប្រាស់ Tag `<audio controls>` ជាមួយឯកសារ `.mp3`។
2. តើហេតុអ្វីបានជាគេតែងតែដាក់ `<source>` ច្រើនជាងមួយនៅខាងក្នុង Tag `<audio>`?
