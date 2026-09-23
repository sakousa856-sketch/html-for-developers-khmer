# មេរៀនទី ២៨៖ ស្តង់ដារ និងច្បាប់សរសេរកូដស្អាត (HTML Style Guide & Best Practices)

> **ការសរសេរកូដឱ្យស្អាត ត្រឹមត្រូវតាមស្តង់ដារ W3C Style Guide ជួយឱ្យកូដងាយស្រួលអាន ងាយស្រួលថែទាំ (Maintain) និងចៀសវាង Bugs។**

---

## គោលការណ៍គ្រឹះទាំង ១០ នៃ HTML Style Guide

### ១. តែងតែប្រកាស `<!DOCTYPE html>` ជានិច្ច
ត្រូវដាក់នៅបន្ទាត់ទី ១ លើគេបង្អស់។

### ២. ប្រើអក្សរតូចលើឈ្មោះ Element និង Attribute (Lowercase Tags & Attributes)
* ✅ ត្រឹមត្រូវ: `<section>`, `<a href="index.html">`
* ❌ មិនគួរប្រើ: `<SECTION>`, `<A HREF="index.html">`

### ៣. បិទ Tag ទាំងអស់ឱ្យបានត្រឹមត្រូវ (Close All HTML Elements)
* ✅ ត្រឹមត្រូវ: `<p>អត្ថបទ</p>`, `<li>ធាតុទី ១</li>`
* ❌ មិនគួរប្រើ: `<p>អត្ថបទ`, `<li>ធាតុទី ១`

### ៤. ដាក់សញ្ញាសម្រង់លើ Attribute Values (Quote Attribute Values)
* ✅ ត្រឹមត្រូវ: `<table class="striped">`, `<input type="text">`
* ❌ មិនគួរប្រើ: `<table class=striped>`

### ៥. កំណត់ `alt`, `width` និង `height` លើរូបភាពជានិច្ច
ជួយការពារ Layout Shift ពេល Browser កំពុង Load រូបភាព។

### ៦. ប្រើគម្លាតដកឃ្លា ២ Spaces សម្រាប់ Indentation
ចៀសវាងការប្រើ Tab ធំៗដែលធ្វើឱ្យកូដលយវែងពិបាកមើល។

```html
<!-- គំរូ Indentation ស្អាត -->
<!DOCTYPE html>
<html lang="km">
  <head>
    <meta charset="UTF-8">
    <title>Style Guide Example</title>
  </head>
  <body>
    <header>
      <h1>ចំណងជើង</h1>
    </header>
  </body>
</html>
```

### ៧. កំណត់ `lang` និង `charset="UTF-8"` ជានិច្ច
ការពារបញ្ហាអក្សរខូចលើភាសាខ្មែរ និងជួយដល់ SEO។

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. យកកូដ HTML ចាស់របស់អ្នកមកពិនិត្យផ្ទៀងផ្ទាត់ឡើងវិញតាមគោលការណ៍ទាំង ៧ ខាងលើ។
2. តើហេតុអ្វីបានជាគេណែនាំឱ្យសរសេរឈ្មោះ Tag ជាអក្សរតូចជានិច្ច?
