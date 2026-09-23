# មេរៀនទី ១០៖ សម្រង់សម្តី និងប្រភព (HTML Quotations & Citations)

> **HTML ផ្តល់នូវ Elements សម្រាប់កំណត់សម្រង់សម្តីខ្លី សម្រង់សម្តីវែង ការបញ្ជាក់ប្រភពអ្នកនិពន្ធ ពាក្យកាត់ និងអាសយដ្ឋាន។**

---

## ១. បណ្តា Quotation Elements ក្នុង HTML

| Tag | ឈ្មោះ | ការប្រើប្រាស់ (Usage) |
| :--- | :--- | :--- |
| `<blockquote>` | Block Quotation | សម្រង់សម្តីវែង (Browser នឹងដកឃ្លា Indent ពីឆ្វេង) |
| `<q>` | Short Inline Quotation | សម្រង់សម្តីខ្លី (Browser នឹងបន្ថែមសញ្ញាសម្រង់ `""` ស្វ័យប្រវត្តិ) |
| `<abbr>` | Abbreviation | ពាក្យកាត់ (បង្ហាញការពន្យល់ពេល hover លើ `title`) |
| `<address>` | Contact Information | ព័ត៌មានទំនាក់ទំនងរបស់អ្នកនិពន្ធ/ម្ចាស់គេហទំព័រ |
| `<cite>` | Title of Work | ឈ្មោះស្នាដៃ ដូចជា សៀវភៅ ភាពយន្ត ចម្រៀង គំនូរ |
| `<bdo>` | Bi-Directional Override | ប្តូរទិសដៅនៃការសរសេរអក្សរ (ឆ្វេងទៅស្តាំ ឬស្តាំទៅឆ្វេង) |

---

## ២. ឧទាហរណ៍កូដជាក់ស្តែង (Code Examples)

### ១. `<blockquote>` និង `<cite>`
```html
<blockquote cite="https://www.w3.org/WAI/">
  "The power of the Web is in its universality. Access by everyone regardless of disability is an essential aspect."
</blockquote>
<p>— សម្រង់សម្តីដោយ <cite>Tim Berners-Lee</cite></p>
```

### ២. `<q>` (សម្រង់ខ្លី)
```html
<p>លោកគ្រូបានមានប្រសាសន៍ថា <q>ការអនុវត្តសរសេរកូដជារៀងរាល់ថ្ងៃ គឺជាគន្លឹះនៃភាពជោគជ័យ</q>។</p>
```

### ៣. `<abbr>` (ពាក្យកាត់)
```html
<p>អង្គការ <abbr title="World Health Organization">WHO</abbr> ត្រូវបានបង្កើតឡើងនៅឆ្នាំ ១៩៤៨។</p>
```

### ៤. `<address>` (អាសយដ្ឋានទំនាក់ទំនង)
```html
<address>
  និពន្ធដោយ៖ លោកគ្រូ សុខ សាន្ត<br>
  ចូលមើលគេហទំព័រ៖ <a href="https://example.com">example.com</a><br>
  រាជធានីភ្នំពេញ ប្រទេសកម្ពុជា
</address>
```

### ៥. `<bdo>` (ប្តូរទិសដៅអក្សរ)
```html
<!-- បង្ហាញអក្សរត្រឡប់ពីស្តាំទៅឆ្វេង (Right-to-Left) -->
<bdo dir="rtl">អត្ថបទនេះនឹងត្រូវអានបញ្ច្រាសទិសដៅ</bdo>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរប្រើប្រាស់ `<abbr>` ដើម្បីពន្យល់ពាក្យកាត់ **CSS** និង **HTML**។
2. បង្កើតប្លុកសម្រង់សម្តី `<blockquote>` មួយដែលអ្នកពេញចិត្ត ដោយមានបញ្ជាក់ឈ្មោះអ្នកនិពន្ធតាមរយៈ `<cite>`។
