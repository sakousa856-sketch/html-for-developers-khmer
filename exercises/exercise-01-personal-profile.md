# 📝 លំហាត់អនុវត្តទី ០១៖ បង្កើតទំព័រព័ត៌មានផ្ទាល់ខ្លួន (Personal Profile)

## 🎯 គោលបំណង (Objective)
អនុវត្តការប្រើប្រាស់រចនាសម្ព័ន្ធមូលដ្ឋាន HTML5, Headings, Paragraphs, Lists, Text Formatting, Images និង Hyperlinks។

---

## 📋 លក្ខខណ្ឌតម្រូវ (Requirements)
សិស្សត្រូវបង្កើត File ឈ្មោះ `profile.html` ដោយមានបញ្ចូលចំណុចដូចខាងក្រោម៖
1. **រចនាសម្ព័ន្ធ HTML5:** មាន `<!DOCTYPE html>`, `<html lang="km">`, `<head>`, `<meta charset="UTF-8">`, `<title>` និង `<body>`។
2. **ចំណងជើងមេ (`<h1>`):** ដាក់ឈ្មោះពេញរបស់អ្នក និងតួនាទី (ឧទាហរណ៍៖ សុខ សាន្ត - Junior Web Developer)។
3. **រូបភាព Profile (`<img>`):** ដាក់រូបថតផ្ទាល់ខ្លួន ឬរូបតំណាង ដោយមានកំណត់ `src`, `alt`, និងទំហំសមរម្យ (`width="200"` ឬ CSS `max-width: 100%`)។
4. **កថាខណ្ឌជីវប្រវត្តិ (`<p>`):** សរសេររៀបរាប់ពីប្រវត្តិរូប និងគោលបំណងក្នុងវិស័យ IT ដោយប្រើប្រាស់ `<b>`, `<strong>`, `<i>`, និង `<mark>`។
5. **បញ្ជីជំនាញ (`<ul>` / `<ol>`):**
   * បញ្ជីរាយចំណាប់អារម្មណ៍ (Unordered List)
   * បញ្ជីរាយគោលដៅ ៣ ឆ្នាំខាងមុខ (Ordered List)
6. **ផ្នែកទំនាក់ទំនង (`<a>`):**
   * Link ទៅកាន់ GitHub ឬ Facebook (បើកក្នុង Tab ថ្មីជាមួយ `target="_blank"`)
   * Link ផ្ញើ Email តាមរយៈ `mailto:`
   * Link ទូរស័ព្ទតាមរយៈ `tel:`

---

## 💡 គន្លឹះជំនួយ (Starter Hint)
```html
<!DOCTYPE html>
<html lang="km">
<head>
  <meta charset="UTF-8">
  <title>ប្រវត្តិរូបរបស់ខ្ញុំ</title>
</head>
<body>
  <h1>ឈ្មោះ៖ ...</h1>
  <img src="..." alt="រូបភាព Profile" width="200">
  <!-- បន្តសរសេរមាតិកាបន្ថែម... -->
</body>
</html>
```
