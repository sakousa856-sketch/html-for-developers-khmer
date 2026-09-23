# មេរៀនទី ២៣៖ ផ្លូវឯកសារ Relative និង Absolute (HTML File Paths)

> **File Path កំណត់ពីទីតាំងឯកសារ (ដូចជា រូបភាព, CSS, JS, HTML Pages ផ្សេងទៀត) នៅក្នុងរចនាសម្ព័ន្ធ Folder នៃគេហទំព័រ។**

---

## ១. ប្រភេទទាំង ២ នៃ File Paths

1. **Absolute File Paths (ផ្លូវដាច់ខាត / URL ពេញលេញ):** ប្រើប្រាស់ពេញលេញពី Protocol រហូតដល់ Domain Name។
2. **Relative File Paths (ផ្លូវធៀប / អាស្រ័យលើទីតាំង File បច្ចុប្បន្ន):** ប្រើសម្រាប់ចង្អុលបង្ហាញ File ក្នុង Folder គម្រោងផ្ទាល់ខ្លួន។

---

## ២. ឧទាហរណ៍ និងរបៀបប្រើ Relative File Paths

![HTML File Paths and Directory Tree](../assets/html-file-paths-tree.svg)

| Syntax | ការពន្យល់ (Meaning) | ឧទាហរណ៍ (Example) |
| :--- | :--- | :--- |
| `picture.jpg` | ឯកសារស្ថិតក្នុង **Folder តែមួយ** ជាមួយ HTML File | `<img src="picture.jpg">` |
| `images/picture.jpg` | ឯកសារស្ថិតក្នុង **Sub-folder** ឈ្មោះ `images` | `<img src="images/picture.jpg">` |
| `/images/picture.jpg` | ឯកសារស្ថិតក្នុង folder `images` នៅ **Root Directory** | `<img src="/images/picture.jpg">` |
| `../picture.jpg` | ថយក្រោយ **១ កម្រិត (One level up)** ទៅកាន់ Parent folder | `<img src="../picture.jpg">` |
| `../../images/pic.jpg` | ថយក្រោយ **២ កម្រិត (Two levels up)** រួចចូល folder `images` | `<img src="../../images/pic.jpg">` |

---

## ៣. ដ្យាក្រាមរចនាសម្ព័ន្ធ Folder គំរូ (Folder Tree Diagram)

```text
my-website/
├── index.html              <-- ហៅរូបភាព: <img src="assets/images/logo.png">
├── style.css
├── assets/
│   └── images/
│       └── logo.png
└── pages/
    └── about.html          <-- ថយក្រោយ ១ កម្រិត: <img src="../assets/images/logo.png">
                            <-- ថយក្រោយ ១ កម្រិត: <link rel="stylesheet" href="../style.css">
```

> [!TIP]
> **ការអនុវត្តល្អ (Best Practice):** ក្នុងការបង្កើត Website ផ្ទាល់ខ្លួន គួរតែប្រើ **Relative File Paths** ជានិច្ច ព្រោះនៅពេលយើងផ្លាស់ប្តូរ Domain ឬ Upload ឡើងទៅ Hosting ផ្សេង វានឹងមិនខូច Link រូបភាព ឬ CSS ឡើយ។

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ប្រសិនបើឯកសារ `contact.html` ស្ថិតក្នុង `my-project/pages/contact.html` ហើយរូបភាពស្ថិតក្នុង `my-project/images/map.png` តើកូដ `src` ត្រូវសរសេរយ៉ាងដូចម្តេច?
2. ចូរពន្យល់ពីភាពខុសគ្នារវាង `src="logo.png"` និង `src="../logo.png"`។
