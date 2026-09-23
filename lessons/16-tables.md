# មេរៀនទី ១៦៖ តារាងទិន្នន័យ (HTML Tables)

> **HTML Tables អនុញ្ញាតឱ្យយើងរៀបចំ និងបង្ហាញទិន្នន័យជាជួរដេក (Rows) និងជួរឈរ (Columns) យ៉ាងមានរបៀប។**

---

## ១. បណ្តា Tags គ្រឹះនៃ Table

| Tag | ឈ្មោះពេញ | តួនាទី (Description) |
| :--- | :--- | :--- |
| `<table>` | Table | Element មេសម្រាប់ក្តោបតារាងទាំងមូល |
| `<tr>` | Table Row | កំណត់ជួរដេកនីមួយៗក្នុងតារាង |
| `<th>` | Table Header | ប្រអប់ចំណងជើងក្បាលតារាង (អក្សរដិត និងចំកណ្តាលស្វ័យប្រវត្តិ) |
| `<td>` | Table Data | ប្រអប់ទិន្នន័យធម្មតាក្នុងតារាង |
| `<thead>` | Table Head | ក្តោបជួរចំណងជើងក្បាលតារាង |
| `<tbody>` | Table Body | ក្តោបជួរទិន្នន័យស្នូល |
| `<tfoot>` | Table Footer | ក្តោបជួរខាងក្រោម (សរុប ឬ Footer) |
| `<caption>` | Table Caption | កំណត់ចំណងជើងពិពណ៌នាតារាង |

---

## ២. ឧទាហរណ៍កូដតារាងស្តង់ដារ (Standard Table Example)

```html
<table border="1" style="border-collapse: collapse; width: 100%;">
  <caption>បញ្ជីឈ្មោះសិស្សពូកែ</caption>
  <thead>
    <tr style="background-color: #0284c7; color: white;">
      <th>លេខរៀង</th>
      <th>ឈ្មោះសិស្ស</th>
      <th>មុខវិជ្ជា</th>
      <th>ពិន្ទុ</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>សុខ សាន្ត</td>
      <td>HTML5 & CSS3</td>
      <td>98</td>
    </tr>
    <tr>
      <td>2</td>
      <td>ចាន់ ធីតា</td>
      <td>JavaScript</td>
      <td>95</td>
    </tr>
  </tbody>
  <tfoot>
    <tr style="background-color: #e2e8f0; font-weight: bold;">
      <td colspan="3" style="text-align: right;">មធ្យមភាគសរុប៖</td>
      <td>96.5</td>
    </tr>
  </tfoot>
</table>
```

---

## ៣. ការបញ្ចូលប្រអប់តារាងចូលគ្នា (Colspan & Rowspan)

* **`colspan="N"` (Column Span):** ពង្រីកប្រអប់មួយឱ្យក្តោបលើ N ជួរឈរ (ផ្តេក)
* **`rowspan="N"` (Row Span):** ពង្រីកប្រអប់មួយឱ្យក្តោបលើ N ជួរដេក (ឈរ)

### ឧទាហរណ៍ `colspan` និង `rowspan`:
```html
<table border="1" style="border-collapse: collapse;">
  <tr>
    <th>ឈ្មោះ</th>
    <th colspan="2">លេខទូរស័ព្ទ (Colspan 2)</th>
  </tr>
  <tr>
    <td>សុខ សាន្ត</td>
    <td>012 345 678</td>
    <td>098 765 432</td>
  </tr>
  <tr>
    <td rowspan="2">ម៉ោងសិក្សា (Rowspan 2)</td>
    <td colspan="2">ព្រឹក៖ 8:00 AM - 11:00 AM</td>
  </tr>
  <tr>
    <td colspan="2">រសៀល៖ 2:00 PM - 5:00 PM</td>
  </tr>
</table>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. ចូរបង្កើតកាលវិភាគប្រចាំសប្តាហ៍ (Timetable) ដោយប្រើប្រាស់ `<table>`, `<thead>`, `<tbody>`, `<th>`, `<td>` និង `colspan/rowspan`។
2. ហេតុអ្វីបានជាគេមិនណែនាំឱ្យប្រើ `<table>` ដើម្បីធ្វើ Layout គេហទំព័រទាំងមូល? (ប្រើ CSS Grid/Flexbox ជំនួសវិញ)។
