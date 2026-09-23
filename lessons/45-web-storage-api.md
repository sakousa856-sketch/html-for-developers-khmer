# មេរៀនទី ៤៥៖ Web Storage API (localStorage & sessionStorage)

> **HTML5 Web Storage API អនុញ្ញាតឱ្យគេហទំព័រអាចផ្ទុកទិន្នន័យ (Key/Value pairs) នៅក្នុង Web Browser របស់អ្នកប្រើប្រាស់ដោយផ្ទាល់ មានសុវត្ថិភាពខ្ពស់ និងផ្ទុកទិន្នន័យបានច្រើនជាង Cookies ចាស់ៗ។**

---

## ១. ភាពខុសគ្នារវាង `localStorage` vs `sessionStorage`

| លក្ខណៈសម្បត្តិ | `window.localStorage` | `window.sessionStorage` |
| :--- | :--- | :--- |
| **អាយុកាលទិន្នន័យ (Expiration)** | **នៅរហូត (No Expiration)** ទោះបីជាបិទ Browser ឬបិទកុំព្យូទ័រ | **បាត់បង់ពេលបិទ Tab ឬបិទ Browser** |
| **ទំហំផ្ទុក (Capacity)** | ប្រហែល 5MB ទៅ 10MB ក្នុងមួយ Domain | ប្រហែល 5MB ក្នុងមួយ Tab |
| **ការប្រើប្រាស់ល្អបំផុត** | Dark Mode Theme, User Preferences, Shopping Cart | Form ទិន្នន័យមួយ Tab, One-time session tokens |

---

## ២. វិធីសាស្ត្រប្រតិបត្តិការសំខាន់ៗ (Methods)

ទាំង `localStorage` និង `sessionStorage` ប្រើប្រាស់ Methods ដូចគ្នាបេះបិទ៖

```javascript
// ១. រក្សាទុកទិន្នន័យ (Set item)
localStorage.setItem('theme', 'dark');

// ២. អានទិន្នន័យមកប្រើ (Get item)
const currentTheme = localStorage.getItem('theme'); // លទ្ធផល: "dark"

// ៣. លុបទិន្នន័យជាក់លាក់មួយ (Remove item)
localStorage.removeItem('theme');

// ៤. លុបទិន្នន័យទាំងអស់ក្នុង Domain នោះចោល (Clear all)
localStorage.clear();
```

---

## ៣. ឧទាហរណ៍ជាក់ស្តែង: ចងចាំ Dark Mode Preference

```html
<!DOCTYPE html>
<html lang="km">
<head>
  <meta charset="UTF-8">
  <title>Dark Mode Demo</title>
  <style>
    body.dark { background: #0f172a; color: white; }
    body.light { background: #f8fafc; color: black; }
  </style>
</head>
<body>

  <h1>សាកល្បងប្តូរ Theme</h1>
  <button onclick="toggleTheme()">🌓 ប្តូរ Dark / Light Mode</button>

  <script>
    // អាន Theme ចាស់ពី localStorage ពេលបើកទំព័រ
    const savedTheme = localStorage.getItem('user_theme') || 'light';
    document.body.className = savedTheme;

    function toggleTheme() {
      const isDark = document.body.classList.contains('dark');
      const newTheme = isDark ? 'light' : 'dark';
      document.body.className = newTheme;
      localStorage.setItem('user_theme', newTheme);
    }
  </script>

</body>
</html>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. តើ `localStorage` និង `sessionStorage` ខុសគ្នាយ៉ាងដូចម្តេច?
2. ចូរបង្កើតកម្មវិធីកត់ត្រាពិន្ទុហ្គេម (High Score Tracker) សាមញ្ញមួយដែលរក្សាទុកពិន្ទុខ្ពស់បំផុតក្នុង `localStorage`។
