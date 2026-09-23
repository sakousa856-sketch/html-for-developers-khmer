# មេរៀនទី ៣០៖ ការកំណត់ Charset និង URL Encoding (HTML Charset & URL Encode)

> **Character Encoding កំណត់ពីរបៀបដែល Browser បម្លែង Bytes ទៅជាតួអក្សរ ហើយ URL Encoding ធានាថាតួអក្សរពិសេសក្នុង URL ត្រូវបានបញ្ជូនឆ្លងកាត់ Internet ដោយសុវត្ថិភាព។**

---

## ១. Character Encoding (`<meta charset="UTF-8">`)

* **ASCII:** គាំទ្រតែតួអក្សរអង់គ្លេស ១២៨ តួអក្សរប៉ុណ្ណោះ។
* **ANSI / Windows-1252:** គាំទ្រតួអក្សរអឺរ៉ុបខាងលិច ២៥៦ តួ។
* **UTF-8 (Unicode Transformation Format - 8-bit):** គាំទ្រតួអក្សរ និងនិមិត្តសញ្ញាស្ទើរតែទាំងអស់នៅលើពិភពលោក រួមទាំង **អក្សរខ្មែរ (Khmer Unicode)**, ចិន, អារ៉ាប់, និង Emojis។

> [!IMPORTANT]
> ត្រូវប្រកាស `<meta charset="UTF-8">` នៅដើមគេក្នុងផ្នែក `<head>` ជានិច្ច ដើម្បីការពារកុំឱ្យ Browser បង្ហាញអក្សរខ្មែរខូច (Mojibake)។

---

## ២. URL Encoding (Percent-Encoding)

URL អាចផ្ទុកបានតែតួអក្សរពីសំណុំ **ASCII Standard** ប៉ុណ្ណោះ។ ប្រសិនបើ URL មានតួអក្សរពិសេស ឬដកឃ្លា (Space) វានឹងត្រូវបម្លែងជាទម្រង់ `%HH` (Hexadecimal)៖

| តួអក្សរដើម (Character) | URL Encoded Result | ការពិពណ៌នា |
| :---: | :---: | :--- |
| ` ` (Space) | `%20` ឬ `+` | ដកឃ្លា |
| `?` | `%3F` | សញ្ញាសួរ (Query String separator) |
| `&` | `%26` | សញ្ញា And (Parameter separator) |
| `/` | `%2F` | Forward slash |
| `:` | `%3A` | Colon |
| `=` | `%3D` | Equals sign |

### ឧទាហរណ៍ជាក់ស្តែង៖
```text
URL ដើម៖  https://example.com/search?query=រៀន html
URL បម្លែង៖ https://example.com/search?query=%E1%9E%9A%E1%9F%8Open%20html
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. តើ UTF-8 មានសារៈសំខាន់យ៉ាងដូចម្តេចចំពោះគេហទំព័រភាសាខ្មែរ?
2. តើដកឃ្លា (Space) នៅក្នុង URL ត្រូវបាន encode ទៅជាអ្វី?
