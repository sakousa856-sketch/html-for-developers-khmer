# 📝 លំហាត់អនុវត្តទី ០៣៖ បង្កើតទម្រង់ស្ទង់មតិសិស្ស (Student Survey Form)

## 🎯 គោលបំណង (Objective)
អនុវត្តការបង្កើត HTML Forms ពេញលេញ ជាមួយ Input Types ទំនើបៗ ការដាក់ Fieldset/Legend និងការធ្វើ Form Validation។

---

## 📋 លក្ខខណ្ឌតម្រូវ (Requirements)
សិស្សត្រូវបង្កើត File ឈ្មោះ `survey.html` ដោយមានបញ្ចូលចំណុចដូចខាងក្រោម៖
1. **Tag `<form>`:** មាន `action="#"` និង `method="POST"`។
2. **Fieldset ទី ១ (ព័ត៌មានទូទៅ):**
   * ប្រអប់ឈ្មោះពេញ (`type="text" required autofocus`)
   * ប្រអប់អ៊ីមែល (`type="email" required`)
   * ប្រអប់លេខទូរស័ព្ទ (`type="tel" pattern="[0-9]{9,10}"`)
   * ប្រអប់កាលបរិច្ឆេទ (`type="date"`)
3. **Fieldset ទី ២ (ការវាយតម្លៃ និងមតិកែលម្អ):**
   * ការវាយតម្លៃគុណភាពបង្រៀន (`type="range" min="1" max="5"`)
   * មុខវិជ្ជាដែលចូលចិត្តជាងគេ (Dropdown `<select>` ឬ `<datalist>`)
   * ការយល់ព្រមលើលក្ខខណ្ឌ (`type="checkbox" required`)
   * ប្រអប់សំណូមពរ (`<textarea rows="4">`)
4. **ប៊ូតុង:**
   * ប៊ូតុង "បញ្ជូនការស្ទង់មតិ" (`type="submit"`)
   * ប៊ូតុង "កំណត់ឡើងវិញ" (`type="reset"`)
