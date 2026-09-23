# មេរៀនទី ០៥៖ លក្ខណៈសម្បត្តិរបស់ធាតុ (HTML Attributes)

> **HTML Attributes ផ្តល់នូវព័ត៌មានបន្ថែម (Additional Information) អំពី Element ហើយតែងតែត្រូវបានកំណត់នៅក្នុង Start Tag ជានិច្ច។**

---

## ១. ទម្រង់ទូទៅនៃ Attribute (Attribute Syntax)

![HTML Attribute Anatomy](../assets/html-attributes-diagram.svg)

Attributes ភាគច្រើនត្រូវបានសរសេរជាទម្រង់ **ឈ្មោះ និងតម្លៃ (name="value")**:

```html
<tagname name="value">Content</tagname>
```

### ឧទាហរណ៍៖
```html
<!-- href គឺជា Attribute របស់ <a> -->
<a href="https://www.google.com">ចូលទៅកាន់ Google</a>

<!-- src និង alt គឺជា Attributes របស់ <img> -->
<img src="logo.png" alt="រូប Logo សាលា" width="200" height="100">
```

---

## ២. បណ្តា Attributes ដែលសំខាន់ និងប្រើញឹកញាប់បំផុត

### ១. `href` Attribute (Hypertext Reference)
ប្រើសម្រាប់កំណត់ URL គោលដៅនៃ Link:
```html
<a href="https://www.w3schools.com">រៀនកូដជាមួយ W3Schools</a>
```

### ២. `src` និង `alt` Attributes
* `src` (Source): ទីតាំង File រូបភាព
* `alt` (Alternative text): អត្ថបទពិពណ៌នារូបភាពពេលរូបភាពមិនទាន់ load ឬសម្រាប់ជនពិការភ្នែកប្រើប្រាស់ Screen Reader
```html
<img src="avatar.jpg" alt="រូប Profile របស់អ្នកប្រើប្រាស់">
```

### ៣. `width` និង `height` Attributes
កំណត់ទំហំទទឹង និងបណ្តោយ (គិតជា Pixels):
```html
<img src="banner.jpg" alt="Banner" width="800" height="400">
```

### ៤. `style` Attribute
ប្រើសម្រាប់កំណត់ CSS Styling ដោយផ្ទាល់លើ Element (Inline CSS) ដូចជា ពណ៌ ទំហំអក្សរ ផ្ទៃខាងក្រោយ:
```html
<p style="color: blue; font-size: 20px;">កថាខណ្ឌអក្សរពណ៌ខៀវ</p>
```

### ៥. `title` Attribute
កំណត់អត្ថបទជំនួយ (Tooltip) ដែលនឹងបង្ហាញឡើងនៅពេលអ្នកប្រើប្រាស់យក Mouse ទៅដាក់លើ (Hover) ធាតុនោះ៖
```html
<p title="នេះជា Tooltip ពន្យល់បន្ថែម">ដាក់ Mouse លើអត្ថបទនេះដើម្បីមើល Tooltip</p>
```

### ៦. `lang` Attribute
កំណត់ភាសាលើ Element ឬលើ `<html>`៖
```html
<html lang="km"> <!-- ភាសាខ្មែរ -->
<html lang="en"> <!-- ភាសាអង់គ្លេស -->
```

---

## ៣. ច្បាប់ និងការអនុវត្តល្អចំពោះ Attributes (Best Practices)

1. **ប្រើអក្សរតូចជានិច្ច (Always use lowercase):** ស្តង់ដារ W3C ណែនាំឱ្យសរសេរឈ្មោះ Attribute ជាអក្សរតូច (ឧ. `href` មិនមែន `HREF`)។
2. **ដាក់ Quote ជានិច្ច (Always quote attribute values):** ត្រូវដាក់សញ្ញាសម្រង់ `""` ជុំវិញ value ជានិច្ច (ឧ. `class="my-box"` មិនមែន `class=my-box`)។

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរពន្យល់ពីសារៈសំខាន់នៃ `alt` attribute ក្នុង Tag `<img>`។
2. បង្កើតតំណភ្ជាប់ `<a>` មួយដែលមាន `href` ទៅកាន់ Facebook និងមាន `title` ថា "ចូលទៅកាន់ទំព័រ Facebook របស់យើង"។
3. បង្កើត Tag `<img>` មួយដែលមានកំណត់ `src`, `alt`, `width` (300px), និង `height` (200px)។
