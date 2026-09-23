# មេរៀនទី ១៨៖ ធាតុ Block និង Inline (HTML Block vs Inline Elements)

> **គ្រប់ HTML Element ទាំងអស់សុទ្ធតែមានតម្លៃបង្ហាញលំនាំដើម (Default Display Value) ជារបៀប Block ឬ Inline។**

---

## ១. ធាតុ Block-level Elements (Block Elements)

### លក្ខណៈពិសេស៖
* **តែងតែចាប់ផ្តើមនៅលើបន្ទាត់ថ្មីជានិច្ច (Always starts on a new line)**
* **ពង្រីកទទឹងពេញ ១០០% នៃទំហំ Parent Container (Takes full width available)**
* អាចកំណត់ `width`, `height`, `margin`, និង `padding` បានពេញលេញ

### បណ្តា Block Elements ដែលនិយមប្រើបំផុត៖
`<div>`, `<h1>` - `<h6>`, `<p>`, `<form>`, `<header>`, `<footer>`, `<section>`, `<article>`, `<nav>`, `<ul>`, `<ol>`, `<li>`, `<table>`, `<blockquote>`, `<hr>`

```html
<!-- Element ទាំងពីរនេះនឹងបង្ហាញលើ ២ បន្ទាត់ដាច់ពីគ្នា -->
<div style="background: lightblue;">ខ្ញុំជា Block Element ទី ១ (ពេញទទឹង)</div>
<div style="background: lightgreen;">ខ្ញុំជា Block Element ទី ២ (ចុះបន្ទាត់ថ្មី)</div>
```

---

## ២. ធាតុ Inline Elements (Inline Elements)

### លក្ខណៈពិសេស៖
* **មិនចុះបន្ទាត់ថ្មីឡើយ (Does not start on a new line)**
* **យកទំហំទទឹងត្រឹមតែប៉ុនទំហំមាតិកាដែលនៅខាងក្នុងប៉ុណ្ណោះ (Takes only necessary width)**
* មិនអាចកំណត់ `width` និង `height` តាម CSS ដោយផ្ទាល់បានទេ (លើកលែងតែប្តូរទៅ `inline-block`)

### បណ្តា Inline Elements ដែលនិយមប្រើបំផុត៖
`<span>`, `<a>`, `<img>`, `<b>`, `<strong>`, `<i>`, `<em>`, `<small>`, `<mark>`, `<label>`, `<input>`, `<button>`, `<code>`

```html
<!-- Elements ទាំងនេះនឹងស្ថិតនៅលើជួរបន្ទាត់តែមួយជាប់គ្នា -->
<p>
  នេះជាអត្ថបទធម្មតា 
  <span style="background: yellow;">ខ្ញុំជា Inline ទី ១</span> 
  <a href="#">ខ្ញុំជា Inline ទី ២</a>
</p>
```

---

## ៣. តារាងប្រៀបធៀបសង្ខេប (Summary Comparison)

| ចំណុចប្រៀបធៀប | Block-level Element | Inline Element |
| :--- | :--- | :--- |
| **ការចុះបន្ទាត់** | ចាប់ផ្តើមបន្ទាត់ថ្មីជានិច្ច | ស្ថិតក្នុងជួរបន្ទាត់ដដែល |
| **ទំហំទទឹង (Width)** | ពង្រីកពេញ 100% | យកតែប៉ុនទំហំ Content |
| **ការដាក់បង្កប់** | អាចផ្ទុក Inline ឬ Block ផ្សេងទៀតបាន | ផ្ទុកបានតែ Text ឬ Inline ផ្សេងទៀត |

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូររៀបរាប់ឈ្មោះ Block Elements ចំនួន ៥ និង Inline Elements ចំនួន ៥។
2. បង្កើតកថាខណ្ឌ `<p>` មួយ រួចប្រើប្រាស់ `<span>` ដែលមានកំណត់ Style ពណ៌ផ្សេង ដើម្បី Highlight ពាក្យចំនួន ២ ក្នុងកថាខណ្ឌនោះ។
