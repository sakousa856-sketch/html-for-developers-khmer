# មេរៀនទី ១៣៖ តំណភ្ជាប់ Hyperlink (HTML Links)

> **HTML Links អនុញ្ញាតឱ្យអ្នកប្រើប្រាស់ចុចផ្លាស់ទីរវាងទំព័រគេហទំព័រ ដោយប្រើប្រាស់ Tag `<a>` (Anchor Tag)។**

---

## ១. ទម្រង់សរសេរ HTML Link (Link Syntax)

```html
<a href="url" target="_blank">អត្ថបទតំណភ្ជាប់ (Link Text)</a>
```

* `href` (Hypertext Reference): កំណត់ URL គោលដៅ។
* អត្ថបទនៅចន្លោះ `<a>` និង `</a>` គឺជាអ្វីដែលអ្នកប្រើប្រាស់មើលឃើញ និងអាចចុចបាន។

---

## ២. Attribute `target` សំខាន់ៗ

Attribute `target` កំណត់ពីរបៀបដែល Browser ត្រូវបើកទំព័រគោលដៅ៖

| Target Value | ការពន្យល់ (Description) |
| :--- | :--- |
| `_self` | (Default) បើកក្នុង Tab/Window ដដែល |
| `_blank` | បើកក្នុង **Tab ឬ Window ថ្មី** |
| `_parent` | បើកក្នុង Parent Frame |
| `_top` | បើកពេញ Window ទាំងមូល (ទម្លុះ Iframes ទាំងអស់) |

> 💡 **ចំណាំសុវត្ថិភាព:** នៅពេលប្រើ `target="_blank"` គួរតែបន្ថែម `rel="noopener noreferrer"` ដើម្បីការពារសុវត្ថិភាព (Tabnabbing attack)។

```html
<a href="https://www.google.com" target="_blank" rel="noopener noreferrer">ចូល Google (Tab ថ្មី)</a>
```

---

## ៣. ប្រភេទនៃតំណភ្ជាប់ផ្សេងៗ (Link Types)

### ១. ប្រើរូបភាពជា Link (Image as Link)
```html
<a href="https://example.com">
  <img src="button.png" alt="ចុចទីនេះ">
</a>
```

### ២. Link ផ្ញើ Email (`mailto:`)
```html
<a href="mailto:support@example.com?subject=ជំនួយបច្ចេកទេស">ទាក់ទងមកផ្នែកបម្រើអតិថិជន</a>
```

### ③. Link ហៅទូរស័ព្ទ (`tel:`)
```html
<a href="tel:+85512345678">ខលមកលេខ +855 12 345 678</a>
```

### ៤. Link លោតទៅកាន់ផ្នែកណាមួយក្នុងទំព័រ (Bookmark / Jump Links)
យើងអាចប្រើ `#id` ដើម្បីឱ្យទំព័រ Scroll ទៅកាន់ Element ដែលមាន `id` នោះភ្លាមៗ៖

```html
<!-- Link នៅផ្នែកខាងលើ -->
<a href="#section-contact">ចុចទៅកាន់ផ្នែកទំនាក់ទំនង</a>

<!-- ខ្លឹមសារវែងៗនៅកណ្តាល... -->

<!-- ផ្នែកគោលដៅនៅខាងក្រោម -->
<h2 id="section-contact">ផ្នែកទំនាក់ទំនង (Contact Us)</h2>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. បង្កើត Link មួយដែលបើកគេហទំព័រ Wikipedia ក្នុង Tab ថ្មី ដោយមានសុវត្ថិភាព `rel="noopener noreferrer"`។
2. បង្កើតប៊ូតុងមួយដែលមានរូបភាព ហើយពេលចុចលើរូបភាពនោះ វានឹងហៅទូរស័ព្ទទៅកាន់លេខរបស់អ្នក។
3. បង្កើតតំណភ្ជាប់ "Scroll to Top" (`#top`) សម្រាប់រំកិលទៅកាន់ផ្នែកខាងលើនៃទំព័រវិញ។
