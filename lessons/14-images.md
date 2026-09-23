# មេរៀនទី ១៤៖ ការប្រើប្រាស់រូបភាព (HTML Images & Picture)

> **Tag `<img>` ត្រូវបានប្រើសម្រាប់បង្កប់រូបភាពទៅក្នុងគេហទំព័រ HTML ដោយវាជា Empty/Void Tag (គ្មាន Closing Tag)។**

---

## ១. ទម្រង់មូលដ្ឋាននៃ Tag `<img>`

```html
<img src="url_or_path" alt="អត្ថបទពិពណ៌នា" width="500" height="300">
```

### Attributes ចាំបាច់ពីរ៖
1. **`src` (Source):** ផ្លូវ ឬ URL នៃរូបភាព។
2. **`alt` (Alternative Text):** អត្ថបទពិពណ៌នារូបភាព (បង្ហាញពេលរូបភាព load មិនចេញ និងជួយដល់ SEO & Screen Readers)។

---

## ២. ទម្រង់រូបភាពដែល Web គាំទ្រ (Supported Image Formats)

| Format | ឈ្មោះពេញ | លក្ខណៈពិសេស (Best For) |
| :--- | :--- | :--- |
| **WebP** | Web Picture format | ណែនាំខ្លាំងបំផុត ⭐ ទំហំស្រាល គុណភាពខ្ពស់ |
| **PNG** | Portable Network Graphics | គាំទ្រផ្ទៃខាងក្រោយថ្លា (Transparent Background), Logo, Icons |
| **JPEG / JPG** | Joint Photographic Experts Group | ស័ក្តិសមសម្រាប់រូបថតទេសភាព មនុស្ស |
| **SVG** | Scalable Vector Graphics | រូបភាពវ៉ិចទ័រ មិនបែកព្រាលពេលពង្រីកធំ |
| **GIF** | Graphics Interchange Format | រូបភាពមានចលនា (Animated image) |
| **AVIF** | AV1 Image File Format | ស្តង់ដារជំនាន់ថ្មី បង្រួមទំហំតូចបំផុត |

---

## ៣. ការគ្រប់គ្រងទំហំ និង Responsive Images

### ១. ប្រើប្រាស់ CSS (ណែនាំដើម្បីកុំឱ្យខូចសមាមាត្ររូបភាព):
```html
<img src="photo.jpg" alt="ទេសភាព" style="width: 100%; max-width: 600px; height: auto;">
```

### ២. ការប្រើប្រាស់ `<picture>` Element
Tag `<picture>` អនុញ្ញាតឱ្យ Browser ជ្រើសរើសរូបភាពខុសៗគ្នាតាមទំហំអេក្រង់ (Responsive Art Direction)៖

```html
<picture>
  <!-- សម្រាប់អេក្រង់កុំព្យូទ័រធំ (Desktop) -->
  <source media="(min-width: 800px)" srcset="banner-large.webp">
  <!-- សម្រាប់ Tablet -->
  <source media="(min-width: 500px)" srcset="banner-medium.webp">
  <!-- រូបភាពលំនាំដើមសម្រាប់ទូរស័ព្ទ (Mobile Fallback) -->
  <img src="banner-small.webp" alt="Banner Promotion" style="width: 100%;">
</picture>
```

### ៣. Performance Optimization ជាមួយ `loading="lazy"`
```html
<!-- Browser នឹងទាញយករូបភាពនេះ លុះត្រាតែអ្នកប្រើប្រាស់ scroll មកជិតដល់ -->
<img src="large-photo.jpg" alt="រូបភាព" loading="lazy">
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរពន្យល់ពីគុណសម្បត្តិនៃការប្រើប្រាស់ `loading="lazy"` លើគេហទំព័រដែលមានរូបភាពច្រើន។
2. បង្កើតទំព័រ HTML មួយដែលមានបង្ហាញរូបភាពចំនួន ៣ ដោយមានកំណត់ `alt`, `style="max-width: 100%; height: auto;"`, និង `loading="lazy"`។
