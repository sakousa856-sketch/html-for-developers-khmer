# មេរៀនទី ២១៖ បង្អួចបង្កប់គេហទំព័រ (HTML Iframes)

> **HTML `<iframe>` (Inline Frame) ត្រូវបានប្រើសម្រាប់បង្កប់គេហទំព័រមួយ ឬមាតិកាខាងក្រៅ (ដូចជា YouTube, Google Maps) ចូលទៅក្នុងគេហទំព័របច្ចុប្បន្ន។**

---

## ១. ទម្រង់សរសេរ Iframe (Iframe Syntax)

```html
<iframe src="url" title="ការពិពណ៌នា" width="100%" height="400"></iframe>
```

* `src`: កំណត់ URL នៃគេហទំព័រ ឬឯកសារដែលត្រូវបង្កប់។
* `title`: ចាំបាច់សម្រាប់ Screen Readers (Accessibility A11y) ដើម្បីដឹងថាមាតិកា Iframe នោះនិយាយអំពីអ្វី។
* `border: none;` (CSS): លុបបន្ទាត់ស៊ុមជុំវិញ frame។

---

## ២. ឧទាហរណ៍ជាក់ស្តែងនៃការប្រើប្រាស់ Iframes

### ១. បង្កប់វីដេអូ YouTube (YouTube Video Embed)
```html
<iframe 
  width="560" 
  height="315" 
  src="https://www.youtube.com/embed/dQw4w9WgXcQ" 
  title="YouTube video player" 
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen>
</iframe>
```

### ២. បង្កប់ផែនទី Google Maps (Google Maps Embed)
```html
<iframe 
  src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15635.848035824962!2d104.9174!3d11.5564" 
  width="600" 
  height="450" 
  style="border:0;" 
  allowfullscreen="" 
  loading="lazy">
</iframe>
```

### ៣. Iframe ជាគោលដៅសម្រាប់ Link (Iframe as Target)
យើងអាចកំណត់ឱ្យ Link បើកទំព័រខាងក្នុង Iframe បាន៖
```html
<iframe src="demo.html" name="myIframe" width="100%" height="300"></iframe>

<p>
  <a href="https://www.w3schools.com" target="myIframe">បើក W3Schools ក្នុង Iframe ខាងលើ</a>
</p>
```

---

## ៣. ចំណុចសុវត្ថិភាព និងការរឹតបន្តឹង (Security & Sandbox)

គេហទំព័រមួយចំនួន (ដូចជា Google Search, Facebook) មិនអនុញ្ញាតឱ្យបង្កប់ក្នុង Iframe ឡើយ ដោយសារគោលការណ៍សុវត្ថិភាព (`X-Frame-Options: SAMEORIGIN`) ដើម្បីការពារការវាយប្រហារ **Clickjacking**។

យើងអាចប្រើប្រាស់ attribute `sandbox` ដើម្បីរឹតបន្តឹងសិទ្ធិរបស់ Iframe៖
```html
<!-- បង្កើនសុវត្ថិភាព ដោយមិនអនុញ្ញាតឱ្យ Iframe ដំណើរការ Script ឬ Submit form ផ្តេសផ្តាស -->
<iframe src="untrusted-page.html" sandbox="allow-scripts allow-same-origin"></iframe>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរចូលទៅកាន់ YouTube រួចជ្រើសរើសវីដេអូណាមួយ ហើយចម្លងកូដ Embed Iframe មកដាក់ក្នុងទំព័រ HTML របស់អ្នក។
2. បង្កើតទំព័រ "ទំនាក់ទំនងយើង" ដោយបង្កប់ផែនទី Google Maps ទីតាំងសាលា ឬផ្ទះរបស់អ្នក។
