# មេរៀនទី ៣៥៖ លក្ខណៈសម្បត្តិរបស់ Input (HTML Input Attributes)

> **Input Attributes កំណត់ពីលក្ខខណ្ឌ កម្រិតកំណត់ ការផ្ទៀងផ្ទាត់ (Validation) និងឥរិយាបថនៃប្រអប់បញ្ចូលទិន្នន័យ។**

---

## ១. បណ្តា Input Attributes សំខាន់ៗបំផុត

| Attribute | ការពន្យល់ (Description) | ឧទាហរណ៍ (Example) |
| :--- | :--- | :--- |
| `value` | តម្លៃទិន្នន័យដំបូងក្នុងប្រអប់ | `value="សុខ"` |
| `readonly` | អាចមើលបាន អាចចម្លងបាន តែ **មិនអាចកែប្រែបាន** | `<input readonly>` |
| `disabled` | បិទមិនឱ្យប្រើប្រាស់ និង **មិនបញ្ជូនទិន្នន័យពេល submit** | `<input disabled>` |
| `placeholder` | អត្ថបទជំនួយពណ៌ប្រផេះស្រាល | `placeholder="វាយឈ្មោះ..."` |
| `required` | ចាំបាច់ត្រូវតែបំពេញ (បើមិនបំពេញ មិនអាច submit បាន) | `<input required>` |
| `autofocus` | ដាក់ Cursor Focus លើប្រអប់នេះស្វ័យប្រវត្តពេលបើកទំព័រ | `<input autofocus>` |
| `maxlength` | ចំនួនតួអក្សរអតិបរមាដែលអាចវាយបាន | `maxlength="10"` |
| `minlength` | ចំនួនតួអក្សរអប្បបរមាដែលតម្រូវឱ្យវាយ | `minlength="6"` |
| `min` / `max` | តម្លៃលេខ ឬកាលបរិច្ឆេទតូចបំផុត / ធំបំផុត | `min="1" max="100"` |
| `step` | ជំហាននៃការកើនឡើងនៃលេខ | `step="5"` (0, 5, 10...) |
| `multiple` | អនុញ្ញាតឱ្យជ្រើសរើស Files ឬ Emails ច្រើនក្នុងពេលតែមួយ | `<input type="file" multiple>` |
| `pattern` | កំណត់ទម្រង់ Regular Expression (Regex) សម្រាប់ផ្ទៀងផ្ទាត់ | `pattern="[0-9]{9,10}"` |

---

## ២. ឧទាហរណ៍ការធ្វើ Form Validation ដោយមិនប្រើ JavaScript

HTML5 អនុញ្ញាតឱ្យយើងធ្វើ Validation យ៉ាងងាយស្រួលតាមរយៈ Attributes៖

```html
<form action="/register" method="POST">
  <!-- តម្រូវឱ្យបំពេញ និងមានប្រវែងយ៉ាងតិច ៣ តួ -->
  <label for="username">ឈ្មោះគណនី (Required, Min 3 chars):</label>
  <input type="text" id="username" name="username" required minlength="3" placeholder="យ៉ាងតិច ៣ តួ"><br><br>

  <!-- កំណត់លេខទូរស័ព្ទកម្ពុជា ៩ ទៅ ១០ ខ្ទង់ ដោយប្រើ Regex Pattern -->
  <label for="phone">លេខទូរស័ព្ទ (Phone):</label>
  <input type="tel" id="phone" name="phone" pattern="[0-9]{9,10}" placeholder="012345678" required><br><br>

  <!-- កំណត់អាយុចន្លោះពី ១៨ ដល់ ៦០ ឆ្នាំ -->
  <label for="age">អាយុ (Age 18 - 60):</label>
  <input type="number" id="age" name="age" min="18" max="60" value="20"><br><br>

  <button type="submit">ចុះឈ្មោះ</button>
</form>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរពន្យល់ពីភាពខុសគ្នារវាង `readonly` និង `disabled`។
2. បង្កើត Form បញ្ចូល Password មួយដែលតម្រូវឱ្យមាន `required`, `minlength="8"`, និង `placeholder="យ៉ាងតិច ៨ តួអក្សរ"`។
