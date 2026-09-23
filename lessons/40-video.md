# មេរៀនទី ៤០៖ វីដេអូក្នុង HTML (HTML Video)

> **Tag `<video>` ក្នុង HTML5 ត្រូវបានប្រើសម្រាប់ចាក់វីដេអូនៅលើគេហទំព័រដោយមិនចាំបាច់ដំឡើង Plugin បន្ថែមឡើយ។**

---

## ១. ទម្រង់សរសេរ HTML Video

```html
<video width="640" height="360" controls poster="thumbnail.jpg">
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.webm" type="video/webm">
  Browser របស់អ្នកមិនគាំទ្រ Video tag ទេ។
</video>
```

---

## ២. បណ្តា Attributes សំខាន់ៗរបស់ `<video>`

| Attribute | ការពន្យល់ (Description) |
| :--- | :--- |
| `controls` | បង្ហាញផ្ទាំងបញ្ជា (ប៊ូតុង Play/Pause, កម្រិតសំឡេង, Fullscreen, Timeline) |
| `autoplay` | ចាក់វីដេអូស្វ័យប្រវត្តពេល load ទំព័រ (តម្រូវឱ្យដាក់ `muted` ទើប Browser អនុញ្ញាត) |
| `muted` | បិទសំឡេងវីដេអូជាមុន |
| `loop` | ចាក់វីដេអូសារឡើងវិញជាប្រចាំមិនចេះចប់ |
| `poster` | កំណត់រូបភាព Thumbnail បង្ហាញមុនពេលវីដេអូត្រូវបានចុច Play |
| `preload` | កំណត់របៀបទាញយកវីដេអូទុកជាមុន (`auto`, `metadata`, `none`) |
| `width` / `height` | កំណត់ទំហំទទឹង និងកម្ពស់នៃ Video Player |

---

## ៣. ការបន្ថែមអក្សររត់ពីក្រោម (Subtitles / Captions) ជាមួយ `<track>`

យើងអាចប្រើប្រាស់ Tag `<track>` ជាមួយឯកសារ WebVTT (`.vtt`) ដើម្បីបន្ថែម Subtitle ជាភាសាខ្មែរ ឬអង់គ្លេស៖

```html
<video width="640" height="360" controls>
  <source src="lesson.mp4" type="video/mp4">
  <track src="subtitles_km.vtt" kind="subtitles" srclang="km" label="ភាសាខ្មែរ" default>
  <track src="subtitles_en.vtt" kind="subtitles" srclang="en" label="English">
</video>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរបង្កើត Video Player មួយដែលមាន `controls`, `poster`, និង `width="100%"` (Responsive)។
2. តើហេតុអ្វីបានជា Browser ភាគច្រើនតម្រូវឱ្យដាក់ `muted` នៅពេលដែលយើងចង់ប្រើ `autoplay`?
