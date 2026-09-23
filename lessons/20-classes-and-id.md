# មេរៀនទី ២០៖ ការប្រើប្រាស់ Class និង ID (HTML Classes & ID)

> **`class` និង `id` គឺជា Global Attributes ដែលប្រើសម្រាប់កំណត់អត្តសញ្ញាណ Element ដើម្បីភ្ជាប់ជាមួយ CSS Styling និង JavaScript Manipulation។**

---

## ១. Attribute `class` (អាចប្រើម្តងហើយម្តងទៀតបាន)

* `class` អាចត្រូវបានកំណត់លើ Elements ជាច្រើនក្នុងទំព័រតែមួយ (Re-usable)
* Element មួយអាចមាន Class ច្រើនជាងមួយ (ខណ្ឌចែកដោយដកឃ្លា)
* ក្នុង CSS យើងហៅ Class ដោយប្រើសញ្ញាចុច (`.classname`)

```html
<!-- HTML -->
<div class="card highlight">កាតទី ១</div>
<div class="card">កាតទី ២</div>
<div class="card">កាតទី ៣</div>

<!-- CSS -->
<style>
  .card {
    padding: 16px;
    border: 1px solid #ddd;
    margin-bottom: 10px;
  }
  .highlight {
    background-color: #fef08a;
  }
</style>
```

---

## ២. Attribute `id` (Unique មួយគត់ក្នុងទំព័រ)

* `id` ត្រូវតែជា **តម្លៃតែមួយគត់ (Unique)** ក្នុងទំព័រ HTML ទាំងមូល (មិនត្រូវដាក់ឈ្មោះ `id` ដូចគ្នាលើសពី ១ Element ឡើយ)
* ក្នុង CSS យើងហៅ ID ដោយប្រើសញ្ញាទ្រង់ជ្រូក (`#idname`)
* ក្នុង JavaScript យើងចាប់យក Element តាមរយៈ `document.getElementById('idname')`
* ប្រើសម្រាប់ធ្វើ Bookmark / Jump Links (`href="#idname"`)

```html
<!-- HTML -->
<h1 id="main-header">ចំណងជើងធំផ្តាច់មុខ</h1>

<!-- CSS -->
<style>
  #main-header {
    color: #0284c7;
    font-size: 32px;
  }
</style>
```

---

## ៣. តារាងប្រៀបធៀបរវាង `class` vs `id`

| លក្ខណៈសម្បត្តិ | `class` Attribute | `id` Attribute |
| :--- | :--- | :--- |
| **ភាពស្ទួន (Uniqueness)** | អាចប្រើស្ទួនលើច្រើន Elements បាន | ត្រូវតែជា **Unique មួយគត់** ក្នុងមួយទំព័រ |
| **ចំនួនលើ Element** | មួយ Element អាចមានច្រើន Class (`class="btn btn-primary"`) | មួយ Element មាន `id` តែមួយគត់ |
| **CSS Selector** | ប្រើសញ្ញាចុច (ឧទាហរណ៍ `.button`) | ប្រើសញ្ញាទ្រង់ជ្រូក (ឧទាហរណ៍ `#submit-btn`) |
| **JavaScript Method** | `document.querySelectorAll('.my-class')` | `document.getElementById('my-id')` |

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរពន្យល់ពីមូលហេតុដែលយើងមិនត្រូវដាក់ឈ្មោះ `id` ដូចគ្នានៅលើ Elements ពីរក្នុងទំព័រតែមួយ។
2. បង្កើតប៊ូតុងចំនួន ៣ ដោយប្រើ Class រួម `.btn` និង Class ពណ៌ផ្សេងគ្នា `.btn-success`, `.btn-danger`, `.btn-warning`។
