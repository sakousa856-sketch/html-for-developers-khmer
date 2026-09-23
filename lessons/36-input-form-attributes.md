# មេរៀនទី ៣៦៖ Form Attributes របស់ Input (HTML Input Form Attributes)

> **Input Form Attributes អនុញ្ញាតឱ្យប៊ូតុង ឬ Input Element ជាក់លាក់មួយ អាច Override (ជំនួស) ការកំណត់របស់ Tag `<form>` មេបាន។**

---

## ១. បណ្តា Input Form Attributes សំខាន់ៗ

| Attribute | តួនាទី (Description) |
| :--- | :--- |
| `form` | កំណត់ថា Input នេះជារបស់ Form ណា (ទោះបីជា Input នោះស្ថិតនៅក្រៅ Tag `<form>` ក៏ដោយ) |
| `formaction` | កំណត់ URL ទទួលទិន្នន័យផ្សេងពី `action` របស់ Form មេ |
| `formenctype` | កំណត់ Encoding ផ្សេងពី `enctype` របស់ Form មេ |
| `formmethod` | កំណត់វិធីសាស្ត្រ HTTP (`GET` ឬ `POST`) ផ្សេងពី `method` របស់ Form មេ |
| `formnovalidate` | បិទ Validation សម្រាប់តែប៊ូតុងមួយនោះប៉ុណ្ណោះ (ឧ. ប៊ូតុង "Save as Draft") |
| `formtarget` | កំណត់ Target ផ្សេងពី `target` របស់ Form មេ |

---

## ២. ឧទាហរណ៍ជាក់ស្តែង (Code Examples)

### ១. ការប្រើប្រាស់ `formaction` និង `formmethod` លើប៊ូតុងផ្សេងគ្នា
```html
<form action="/submit-normal" method="POST" id="mainForm">
  <label for="title">ចំណងជើងអត្ថបទ:</label>
  <input type="text" id="title" name="title" required><br><br>

  <!-- ប៊ូតុង Submit ធម្មតា (ទៅកាន់ /submit-normal) -->
  <button type="submit">ចុះផ្សាយជាសាធារណៈ (Publish)</button>

  <!-- ប៊ូតុងរក្សាទុកព្រាង (ទៅកាន់ /save-draft ដោយមិនបាច់ Validate) -->
  <button type="submit" formaction="/save-draft" formnovalidate>រក្សាទុកជាព្រាង (Save Draft)</button>
</form>
```

### ២. ការប្រើប្រាស់ Attribute `form` លើ Input នៅក្រៅ Form
```html
<!-- Form នៅផ្នែកខាងលើ -->
<form action="/login" method="POST" id="loginForm">
  <input type="text" name="username" placeholder="ឈ្មោះគណនី">
</form>

<!-- ប្រអប់ Password ស្ថិតនៅកន្លែងផ្សេងក្នុង Layout ប៉ុន្តែភ្ជាប់ជាមួយ loginForm តាមរយៈ attribute form -->
<p>ខ្លឹមសារផ្សេងៗ...</p>
<input type="password" name="password" placeholder="ពាក្យសម្ងាត់" form="loginForm">
<button type="submit" form="loginForm">Login</button>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរបង្កើត Form មួយដែលមានប៊ូតុង ២: ប៊ូតុងទី ១ គឺ "Submit Normal" ហើយប៊ូតុងទី ២ គឺ "Save Draft" ដោយប្រើ `formnovalidate` និង `formaction`។
2. សាកល្បងដាក់ Input មួយនៅក្រៅ Tag `<form>` រួចភ្ជាប់វាដោយប្រើ attribute `form="form_id"`។
