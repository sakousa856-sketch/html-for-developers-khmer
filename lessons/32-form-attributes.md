# មេរៀនទី ៣២៖ លក្ខណៈសម្បត្តិនៃ Form (HTML Form Attributes)

> **Form Attributes កំណត់ពីរបៀបដែល Form ត្រូវផ្ញើទិន្នន័យ ទីតាំងគោលដៅ និងវិធីសាស្ត្របញ្ជូន (HTTP Methods)។**

---

## ១. បណ្តា Form Attributes សំខាន់ៗ

| Attribute | ការពន្យល់ (Description) |
| :--- | :--- |
| `action` | កំណត់ URL ឬ File លើ Server ដែលត្រូវទទួលទិន្នន័យពី Form (ឧ. `action="/api/register"`) |
| `method` | កំណត់វិធីសាស្ត្រ HTTP Request (`GET` ឬ `POST`) |
| `target` | កំណត់កន្លែងបង្ហាញលទ្ធផលក្រោយ submit (`_blank`, `_self`) |
| `autocomplete` | បើក (`on`) ឬបិទ (`off`) មុខងារចងចាំទិន្នន័យស្វ័យប្រវត្តិរបស់ Browser |
| `novalidate` | បិទការផ្ទៀងផ្ទាត់ HTML5 Default Validation (សម្រាប់ Custom JS Validation) |
| `enctype` | កំណត់ទម្រង់ Encoding នៃទិន្នន័យ (ចាំបាច់ត្រូវប្រើ `multipart/form-data` ពេល upload files) |

---

## ២. ភាពខុសគ្នារវាង HTTP Methods: `GET` vs `POST`

### 🔹 វិធីសាស្ត្រ `GET` (Default)
* ទិន្នន័យទាំងអស់នឹងត្រូវបង្ហាញនៅលើ **URL Address Bar** ក្នុងទម្រង់ Name/Value pairs (`/search?q=html&page=1`)
* មានកម្រិតប្រវែងទិន្នន័យ (អតិបរមាប្រហែល 2048 តួអក្សរ)
* អាច Bookmark និង Share URL បាន
* **ហាមប្រើសម្រាប់ទិន្នន័យសម្ងាត់** (ដូចជា Password ឬ Credit Card)
* **ស័ក្តិសមសម្រាប់:** ការស្វែងរកទិន្នន័យ (Search Queries)

### 🔹 វិធីសាស្ត្រ `POST`
* ទិន្នន័យត្រូវបានបង្កប់នៅក្នុង **HTTP Request Body** (មិនបង្ហាញលើ URL ឡើយ)
* គ្មានកម្រិតទំហំទិន្នន័យទេ (អាចផ្ញើឯកសារធំៗ ឬ Upload Files បាន)
* មិនអាច Bookmark បានទេ
* **ស័ក្តិសមសម្រាប់:** ការចុះឈ្មោះ, ការ Login, ការកែប្រែទិន្នន័យ ឬការផ្ញើព័ត៌មានរសើប

---

## ៣. ឧទាហរណ៍ Form Upload File ជាមួយ `enctype`

```html
<form action="/upload" method="POST" enctype="multipart/form-data">
  <label for="avatar">ជ្រើសរើសរូបភាព Profile:</label>
  <input type="file" id="avatar" name="avatar" accept="image/*">
  <button type="submit">Upload រូបភាព</button>
</form>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. តើនៅពេលណាដែលយើងត្រូវប្រើប្រាស់ method `GET` ហើយពេលណាត្រូវប្រើ `POST`?
2. ចូរបង្កើត Form ស្វែងរក (Search Form) ដែលប្រើ `action="https://www.google.com/search"` និង `method="GET"` ដោយមាន input ឈ្មោះ `q`។ សាកល្បងចុច Submit ដើម្បីតេស្តលទ្ធផល។
