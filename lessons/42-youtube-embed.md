# មេរៀនទី ៤២៖ ការបង្កប់វីដេអូ YouTube (HTML YouTube Embed)

> **វិធីងាយស្រួល និងពេញនិយមបំផុតក្នុងការចាក់វីដេអូលើគេហទំព័រ គឺការបង្កប់ (Embed) វីដេអូពី YouTube ដោយប្រើប្រាស់ Tag `<iframe>`។**

---

## ១. របៀបបង្កប់វីដេអូ YouTube (How to Embed)

### ជំហានអនុវត្ត៖
1. បើកវីដេអូនៅលើ YouTube ក្នុង Browser
2. ចុចលើប៊ូតុង **Share** រួចជ្រើសរើស **Embed**
3. ចម្លង (Copy) កូដ HTML មកបិទភ្ជាប់ (Paste) ក្នុងឯកសារ HTML របស់អ្នក

```html
<iframe 
  width="560" 
  height="315" 
  src="https://www.youtube.com/embed/M7lc1UVf-VE" 
  title="YouTube video player" 
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
  allowfullscreen>
</iframe>
```

---

## ២. បណ្តា Parameters សំខាន់ៗរបស់ YouTube URL

យើងអាចបន្ថែម Parameters ទៅខាងចុងនៃ URL (`?param1=value&param2=value`) ដើម្បីបញ្ជា YouTube Player៖

| Parameter | ការកំណត់ (Usage) | ឧទាហរណ៍ (Example) |
| :--- | :--- | :--- |
| `autoplay=1` | ចាក់វីដេអូស្វ័យប្រវត្តិ (ត្រូវភ្ជាប់ជាមួយ `mute=1`) | `src="https://.../embed/VIDEO_ID?autoplay=1&mute=1"` |
| `mute=1` | បិទសំឡេងវីដេអូជាមុន | `src="https://.../embed/VIDEO_ID?mute=1"` |
| `controls=0` | លាក់ផ្ទាំងបញ្ជារបស់ YouTube Player | `src="https://.../embed/VIDEO_ID?controls=0"` |
| `loop=1` | ចាក់វិលជុំឡើងវិញ (តម្រូវឱ្យដាក់ `playlist=VIDEO_ID`) | `src="https://.../embed/VIDEO_ID?loop=1&playlist=VIDEO_ID"` |

---

## ៣. ការធ្វើឱ្យ YouTube Iframe មានលក្ខណៈ Responsive (16:9 Aspect Ratio)

```html
<style>
  .video-responsive {
    position: relative;
    padding-bottom: 56.25%; /* សមាមាត្រ 16:9 */
    height: 0;
    overflow: hidden;
    max-width: 100%;
    border-radius: 8px;
  }
  .video-responsive iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
</style>

<div class="video-responsive">
  <iframe src="https://www.youtube.com/embed/M7lc1UVf-VE" allowfullscreen></iframe>
</div>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរជ្រើសរើសវីដេអូបទចម្រៀង ឬមេរៀនមួយពី YouTube រួចបង្កប់វាចូលក្នុងគេហទំព័ររបស់អ្នក។
2. បង្កើត Responsive Video Container តាមគំរូ CSS ខាងលើ ដើម្បីឱ្យវីដេអូបង្ហាញសមាមាត្រស្អាតទាំងលើទូរស័ព្ទដៃ និងកុំព្យូទ័រ។
