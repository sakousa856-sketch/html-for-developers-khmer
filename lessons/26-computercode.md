# មេរៀនទី ២៦៖ ធាតុបង្ហាញកូដកុំព្យូទ័រ (HTML Computer Code Elements)

> **HTML ផ្តល់នូវ Elements ពិសេសសម្រាប់បង្ហាញកូដកុំព្យូទ័រ ប៊ូតុងក្ដារចុច (Keyboard Input) អថេរ និងលទ្ធផលកម្មវិធី។**

---

## ១. បណ្តា Computer Code Elements ក្នុង HTML

| Tag | ឈ្មោះ | ការប្រើប្រាស់ (Usage) |
| :--- | :--- | :--- |
| `<code>` | Inline Code | បង្ហាញកូដកុំព្យូទ័រខ្លីៗក្នុងបន្ទាត់ (Inline Code Snippet) |
| `<kbd>` | Keyboard Input | បង្ហាញប៊ូតុងក្ដារចុចដែលអ្នកប្រើប្រាស់ត្រូវចុច (ឧ. Ctrl + C) |
| `<samp>` | Sample Output | បង្ហាញលទ្ធផលចេញពីកម្មវិធីកុំព្យូទ័រ (Computer Output) |
| `<var>` | Variable | បង្ហាញអថេរគណិតវិទ្យា ឬអថេរក្នុងកូដ (Math / Programming Variable) |
| `<pre>` | Preformatted Text | ប្រើសម្រាប់ក្តោបកូដច្រើនបន្ទាត់ដោយរក្សាទុកគម្លាត Spaces និង Indents |

---

## ២. ឧទាហរណ៍កូដជាក់ស្តែង (Code Examples)

### ១. ការប្រើប្រាស់ `<code>` ជាមួយ `<pre>` (សម្រាប់ Code Block ធំៗ)
```html
<pre>
<code>
function calculateTotal(price, tax) {
  return price + (price * tax);
}
</code>
</pre>
```

### ២. ការប្រើប្រាស់ `<kbd>` (ប៊ូតុង Shortcut)
```html
<p>ដើម្បីចម្លងកូដ សូមចុច <kbd>Ctrl</kbd> + <kbd>C</kbd> (ឬ <kbd>Cmd</kbd> + <kbd>C</kbd> លើ Mac)។</p>
```

### ៣. ការប្រើប្រាស់ `<samp>` និង `<var>`
```html
<p>សមីការបន្ទាត់ត្រង់៖ <var>y</var> = <var>m</var><var>x</var> + <var>b</var></p>

<p>លទ្ធផលចេញពី Server៖ <samp>200 OK - Connected Successfully</samp></p>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរសរសេរការណែនាំអំពីរបៀប Save File ក្នុង VS Code ដោយប្រើប្រាស់ Tag `<kbd>`។
2. បង្កើតប្លុកបង្ហាញកូដ HTML មួយដោយប្រើប្រាស់ការរួមបញ្ចូលគ្នារវាង `<pre>` និង `<code>`។
