# មេរៀនទី ៣៤៖ ប្រភេទនៃ Input ទាំងអស់ (HTML Input Types)

> **Attribute `type` លើ Tag `<input>` កំណត់ពីទម្រង់ និងប្រភេទនៃទិន្នន័យដែលអ្នកប្រើប្រាស់អាចបញ្ចូលបាន។ HTML5 បានបន្ថែម Input Types ឆ្លាតវៃជាច្រើន។**

---

## ១. តារាង Input Types ទាំងអស់ក្នុង HTML5

| Input Type | រូបរាង / មុខងារ (Functionality) | ការផ្ទៀងផ្ទាត់ (Validation) |
| :--- | :--- | :--- |
| `type="text"` | ប្រអប់បញ្ចូលអត្ថបទធម្មតាមួយជួរ | ធម្មតា |
| `type="password"` | លាក់តួអក្សរជាសញ្ញាចុចៗ (`••••••`) | ការពារការលួចមើល Password |
| `type="email"` | សម្រាប់វាយ Email Address | ផ្ទៀងផ្ទាត់សញ្ញា `@` និង Domain ស្វ័យប្រវត្តិ |
| `type="number"` | សម្រាប់តែបញ្ចូលលេខសុទ្ធសាធ | មានប៊ូតុងឡើងចុះ និង validation លេខ |
| `type="tel"` | សម្រាប់លេខទូរស័ព្ទ (Phone Number) | បង្ហាញ Numeric Keypad លើទូរស័ព្ទ |
| `type="url"` | សម្រាប់វាយគេហទំព័រ (`https://...`) | ផ្ទៀងផ្ទាត់ទម្រង់ URL ស្វ័យប្រវត្តិ |
| `type="search"` | ប្រអប់ស្វែងរក | មានសញ្ញា `x` សម្រាប់លុបអក្សរលឿន |
| `type="date"` | ប្រអប់ជ្រើសរើសថ្ងៃខែឆ្នាំ | បង្ហាញប្រតិទិន (Calendar Picker) |
| `type="time"` | ប្រអប់ជ្រើសរើសម៉ោង នាទី | បង្ហាញ Time Picker |
| `type="datetime-local"` | ជ្រើសរើសទាំងថ្ងៃ និងម៉ោង | Date & Time Picker |
| `type="color"` | ប្រអប់ជ្រើសរើសពណ៌ | បង្ហាញ Color Palette Picker |
| `type="range"` | របារអូសជ្រើសរើសតម្លៃ (Slider) | កំណត់ min/max/step |
| `type="checkbox"` | ប្រអប់ធីក (អាចរើសបានច្រើន) | Checkbox Square |
| `type="radio"` | រង្វង់ធីក (រើសបានតែ ១ គត់ក្នុងមួយក្រុម) | Radio Circle |
| `type="file"` | ប៊ូតុងជ្រើសរើសឯកសារសម្រាប់ Upload | File Chooser Dialog |
| `type="hidden"` | លាក់ទិន្នន័យមិនឱ្យអ្នកប្រើប្រាស់ឃើញ | សម្រាប់ផ្ញើ ID/Token ទៅ Server |
| `type="submit"` | ប៊ូតុងបញ្ជូន Form | Submit Button |
| `type="reset"` | ប៊ូតុងលុបទិន្នន័យក្នុង Form ឡើងវិញ | Reset Button |
| `type="button"` | ប៊ូតុងចុចធម្មតាសម្រាប់ JavaScript | Regular Button |

---

## ២. ឧទាហរណ៍ជាក់ស្តែង (Code Examples)

```html
<!-- Radio Buttons (ជ្រើសរើសបានតែមួយគត់ ព្រោះមាន name ដូចគ្នា) -->
<p>ជ្រើសរើសភេទរបស់អ្នក:</p>
<input type="radio" id="male" name="gender" value="male">
<label for="male">ប្រុស</label>
<input type="radio" id="female" name="gender" value="female">
<label for="female">ស្រី</label>

<!-- Checkboxes (ជ្រើសរើសបានច្រើន) -->
<p>យានជំនិះដែលអ្នកមាន:</p>
<input type="checkbox" id="bike" name="vehicle1" value="Bike">
<label for="bike">កង់</label>
<input type="checkbox" id="car" name="vehicle2" value="Car">
<label for="car">រថយន្ត</label>

<!-- Color & Range Pickers -->
<label for="favcolor">ពណ៌ដែលចូលចិត្ត:</label>
<input type="color" id="favcolor" name="favcolor" value="#0284c7"><br><br>

<label for="volume">កម្រិតសំឡេង (០ ដល់ ១០០):</label>
<input type="range" id="volume" name="volume" min="0" max="100">
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរបង្កើត Form មួយដែលមាន `type="email"`, `type="password"`, `type="date"`, `type="color"`, និង `type="range"`។
2. សាកល្បងចុច Submit លើ Form ដោយមិនវាយសញ្ញា `@` ក្នុងប្រអប់ email ហើយកត់ត្រាពីសារ Error ដែល Browser បង្ហាញ។
