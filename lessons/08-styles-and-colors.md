# មេរៀនទី ០៨៖ ការកំណត់ Style និងពណ៌ (HTML Styles & Colors)

> **Attribute `style` ត្រូវបានប្រើដើម្បីបន្ថែមការរចនា (CSS Styling) ដោយផ្ទាល់លើ HTML Element ដូចជា ពណ៌អក្សរ ផ្ទៃខាងក្រោយ ទំហំអក្សរ និងការតម្រឹមកថាខណ្ឌ។**

---

## ១. ទម្រង់សរសេរ HTML Style (Style Syntax)

```html
<tagname style="property: value;">Content</tagname>
```

---

## ២. លក្ខណៈសម្បត្តិ CSS Style សំខាន់ៗ (Core Style Properties)

### ១. ពណ៌ផ្ទៃខាងក្រោយ (`background-color`)
```html
<body style="background-color: #f8fafc;">
  <h1 style="background-color: dodgerblue; color: white;">ចំណងជើងមានផ្ទៃខាងក្រោយពណ៌ខៀវ</h1>
</body>
```

### ២. ពណ៌អក្សរ (`color`)
```html
<p style="color: crimson;">កថាខណ្ឌនេះមានអក្សរពណ៌ក្រហម។</p>
```

### ៣. ពុម្ពអក្សរ (`font-family`)
```html
<p style="font-family: 'Kantumruy Pro', sans-serif;">អត្ថបទប្រើពុម្ពអក្សរ Kantumruy Pro</p>
```

### ៤. ទំហំអក្សរ (`font-size`)
```html
<h1 style="font-size: 300%;">ចំណងជើងទំហំធំខ្លាំង</h1>
<p style="font-size: 18px;">កថាខណ្ឌទំហំ 18px</p>
```

### ៥. ការតម្រឹមអត្ថបទ (`text-align`)
```html
<h1 style="text-align: center;">ចំណងជើងនៅចំកណ្តាល (Centered Heading)</h1>
<p style="text-align: right;">អត្ថបទតម្រឹមខាងស្តាំ (Right Aligned)</p>
```

---

## ៣. ប្រព័ន្ធកំណត់ពណ៌ក្នុង HTML (HTML Color Formats)

HTML គាំទ្រការកំណត់ពណ៌តាម ៤ ទម្រង់ស្តង់ដារ៖

| ប្រព័ន្ធពណ៌ (Format) | ឧទាហរណ៍ (Example) | ការពន្យល់ (Description) |
| :--- | :--- | :--- |
| **Color Names** | `red`, `blue`, `tomato`, `seagreen` | ឈ្មោះពណ៌ស្តង់ដារ ១៤០ ពណ៌ក្នុង HTML |
| **HEX Values** | `#ff0000`, `#0284c7`, `#1e293b` | លេខកូដគោលដប់ប្រាំមួយ (Hexadecimal `#RRGGBB`) |
| **RGB Values** | `rgb(255, 99, 71)` | តម្លៃក្រហម បៃតង ខៀវ (០ ដល់ ២៥៥) |
| **RGBA Values** | `rgba(2, 132, 199, 0.5)` | RGB បន្ថែម Alpha (ភាពថ្លា/Opacity ពី 0 ដល់ 1) |
| **HSL Values** | `hsl(200, 100%, 50%)` | Hue (ដឺក្រេ), Saturation (%), Lightness (%) |

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរបង្កើតកថាខណ្ឌ `<p>` មួយដែលមានផ្ទៃខាងក្រោយពណ៌ប្រផេះស្រាល (`#f1f5f9`), ពណ៌អក្សរខៀវ (`#0369a1`), និងទំហំអក្សរ `20px`។
2. បង្កើត `<h2>` មួយដែលមានអត្ថបទនៅចំកណ្តាល (`text-align: center`) និងមានពណ៌អក្សរជាកូដ RGB `rgb(220, 38, 38)`។
