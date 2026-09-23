# មេរៀនទី ៣១៖ សេចក្តីណែនាំអំពី HTML Forms (HTML Forms Introduction)

> **HTML Form ត្រូវបានប្រើសម្រាប់ប្រមូលទិន្នន័យពីអ្នកប្រើប្រាស់ (User Input) ដូចជា ការចុះឈ្មោះ Login ការស្វែងរក និងបញ្ជូនវាទៅកាន់ Server សម្រាប់ដំណើរការ។**

---

## ១. រចនាសម្ព័ន្ធគ្រឹះនៃ Tag `<form>`

![HTML Form Anatomy and Data Flow](../assets/html-form-anatomy.svg)

```html
<form action="/submit-data" method="POST">
  <label for="fname">ឈ្មោះដំបូង (First Name):</label><br>
  <input type="text" id="fname" name="fname" value="សុខ"><br><br>

  <label for="lname">នាមត្រកូល (Last Name):</label><br>
  <input type="text" id="lname" name="lname" value="សាន្ត"><br><br>

  <input type="submit" value="បញ្ជូនទិន្នន័យ (Submit)">
</form>
```

---

## ២. សារៈសំខាន់នៃ Tag `<label>` និង Attribute `for`

Tag `<label>` កំណត់ឈ្មោះសម្គាល់សម្រាប់ Form Control នីមួយៗ៖
* **Accessibility:** ជួយដល់ Screen Readers ក្នុងការអានឈ្មោះប្រអប់ input ឱ្យអ្នកប្រើប្រាស់ដឹង។
* **User Experience (UX):** នៅពេលអ្នកប្រើប្រាស់ចុច Mouse លើអក្សរនៃ `<label>` វានឹង Focus លើប្រអប់ `<input>` ដោយស្វ័យប្រវត្តិ (ជាពិសេសលើ Checkbox និង Radio)។
* **ការភ្ជាប់ទំនាក់ទំនង:** តម្លៃនៃ `for` ក្នុង `<label>` ត្រូវតែ **ដូចគ្នាបេះបិទនឹង `id`** នៃ `<input>`។

---

## ៣. សារៈសំខាន់នៃ Attribute `name`

> [!WARNING]
> ប្រសិនបើ Tag `<input>` **គ្មាន Attribute `name` ទេ** នោះទិន្នន័យក្នុងប្រអប់នោះ **នឹងមិនត្រូវបានបញ្ជូន (Submitted) ទៅកាន់ Server ឡើយ!**

```html
<!-- ✅ ត្រឹមត្រូវ: ទិន្នន័យឈ្មោះនឹងត្រូវផ្ញើទៅ Server ជា "username=soksan" -->
<input type="text" id="username" name="username">

<!-- ❌ ខុស: គ្មាន attribute name ទេ ទិន្នន័យនឹងត្រូវបាត់បង់ពេល submit -->
<input type="text" id="username">
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរពន្យល់ពីតួនាទីរបស់ `<label for="...">` និងសារៈសំខាន់នៃ attribute `name` ក្នុង Tag `<input>`។
2. បង្កើត Login Form សាមញ្ញមួយដែលមានប្រអប់បញ្ចូល Email, Password និងប៊ូតុង Login។
