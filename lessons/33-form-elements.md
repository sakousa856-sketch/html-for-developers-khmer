# មេរៀនទី ៣៣៖ ធាតុផ្សេងៗក្នុង Form (HTML Form Elements)

> **ក្រៅពី Tag `<input>` ធម្មតា HTML Form មាន Elements ជាច្រើនទៀតសម្រាប់បង្កើតជម្រើស Dropdown, Textarea, Fieldset, Datalist និង Buttons។**

---

## ១. បណ្តា Form Elements ទាំងអស់ក្នុង HTML

| Tag | ឈ្មោះ | ការប្រើប្រាស់ (Usage) |
| :--- | :--- | :--- |
| `<input>` | Input Field | ប្រអប់បញ្ចូលទិន្នន័យទូទៅ |
| `<label>` | Label | ឈ្មោះសម្គាល់ប្រអប់ Input |
| `<select>` | Dropdown List | បញ្ជីជម្រើសទម្លាក់ចុះ (Dropdown) |
| `<option>` | Option Item | ជម្រើសនីមួយៗក្នុង `<select>` ឬ `<datalist>` |
| `<optgroup>` | Option Group | ប្រមូលផ្តុំក្រុមនៃ Options ក្នុង Dropdown |
| `<textarea>` | Multi-line Text Field | ប្រអប់វាយបញ្ចូលអត្ថបទច្រើនបន្ទាត់ (Comments, Messages) |
| `<button>` | Clickable Button | ប៊ូតុងចុច (Submit, Reset, Button) |
| `<fieldset>` | Form Group Box | ប្រអប់គូសស៊ុមជុំវិញក្រុមទិន្នន័យ |
| `<legend>` | Fieldset Caption | ចំណងជើងនៃ `<fieldset>` |
| `<datalist>` | Autocomplete List | បញ្ជីផ្តល់ជម្រើសស្វ័យប្រវត្តិតាមការវាយអក្សរ |
| `<output>` | Calculation Result | បង្ហាញលទ្ធផលនៃការគណនា |

---

## ២. ឧទាហរណ៍កូដជាក់ស្តែង (Code Examples)

### ១. Dropdown List ជាមួយ `<select>` និង `<optgroup>`
```html
<label for="car">ជ្រើសរើសរថយន្ត:</label>
<select id="car" name="car">
  <optgroup label="រថយន្តអគ្គិសនី (EV)">
    <option value="tesla">Tesla Model Y</option>
    <option value="byd">BYD Seal</option>
  </optgroup>
  <optgroup label="រថយន្តសាំង">
    <option value="toyota">Toyota Prius</option>
    <option value="ford">Ford Ranger</option>
  </optgroup>
</select>
```

### ២. ប្រអប់អត្ថបទច្រើនបន្ទាត់ `<textarea>`
```html
<label for="feedback">មតិកែលម្អ (Feedback):</label><br>
<textarea id="feedback" name="feedback" rows="4" cols="50" placeholder="សូមសរសេរមតិរបស់អ្នកនៅទីនេះ..."></textarea>
```

### ៣. ការប្រើប្រាស់ `<fieldset>` និង `<legend>`
```html
<fieldset>
  <legend>ព័ត៌មានអត្តសញ្ញាណ (Identity)</legend>
  <label for="name">ឈ្មោះ:</label>
  <input type="text" id="name" name="name"><br><br>
  <label for="nid">លេខអត្តសញ្ញាណប័ណ្ណ:</label>
  <input type="text" id="nid" name="nid">
</fieldset>
```

### ៤. Autocomplete List ជាមួយ `<datalist>`
```html
<label for="browser">ជ្រើសរើស Browser ដែលអ្នកចូលចិត្ត:</label>
<input list="browsers" id="browser" name="browser">

<datalist id="browsers">
  <option value="Google Chrome">
  <option value="Mozilla Firefox">
  <option value="Apple Safari">
  <option value="Microsoft Edge">
  <option value="Brave">
</datalist>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរបង្កើត Dropdown List `<select>` ដែលអនុវត្តការជ្រើសរើសមុខវិជ្ជា ដោយមានបែងចែកជា ២ ក្រុមតាមរយៈ `<optgroup>`។
2. បង្កើត Form ទំនាក់ទំនងដែលមាន `<fieldset>`, `<legend>`, `<input>`, `<textarea>`, និង `<button>`។
