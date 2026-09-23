# មេរៀនទី ៤៤៖ Drag and Drop API (ការអូសទម្លាក់)

> **HTML5 Drag and Drop API អនុញ្ញាតឱ្យអ្នកប្រើប្រាស់អាចចុច Mouse អូស Element មួយ (Drag) ទៅទម្លាក់ (Drop) លើ Element មួយផ្សេងទៀតនៅលើគេហទំព័រ។**

---

## ១. ជំហានទាំង ៣ នៃការបង្កើត Drag and Drop

1. **ធ្វើឱ្យ Element អាចអូសបាន:** កំណត់ attribute `draggable="true"` លើ Element។
2. **ចាប់ព្រឹត្តិការណ៍ចាប់ផ្តើមអូស (`ondragstart`):** កំណត់ទិន្នន័យដែលត្រូវផ្ទេរតាមរយៈ `dataTransfer.setData()`។
3. **អនុញ្ញាតឱ្យទម្លាក់បាន (`ondragover` និង `ondrop`):** ហៅ `event.preventDefault()` ក្នុង `ondragover` ដើម្បីឱ្យ Browser អនុញ្ញាតការទម្លាក់។

---

## ២. ឧទាហរណ៍កូដជាក់ស្តែង (Complete Example)

```html
<!DOCTYPE html>
<html lang="km">
<head>
  <meta charset="UTF-8">
  <title>Drag and Drop Demo</title>
  <style>
    .drop-box {
      width: 250px;
      height: 150px;
      padding: 10px;
      border: 2px dashed #0284c7;
      border-radius: 8px;
      display: inline-block;
      vertical-align: top;
      margin-right: 20px;
      background: #f8fafc;
    }
    .drag-item {
      width: 120px;
      padding: 12px;
      background: #0284c7;
      color: white;
      text-align: center;
      border-radius: 6px;
      cursor: grab;
    }
  </style>
</head>
<body>

  <h2>សាកល្បងអូសប្រអប់ខាងក្រោមទៅទម្លាក់ក្នុងប្រអប់ទី ២</h2>

  <!-- ប្រអប់ទម្លាក់ទី ១ -->
  <div class="drop-box" ondrop="drop(event)" ondragover="allowDrop(event)">
    <div id="drag1" class="drag-item" draggable="true" ondragstart="drag(event)">
      📦 អូសខ្ញុំ (Drag Me)
    </div>
  </div>

  <!-- ប្រអប់ទម្លាក់ទី ២ -->
  <div class="drop-box" ondrop="drop(event)" ondragover="allowDrop(event)"></div>

  <script>
    function allowDrop(ev) {
      ev.preventDefault(); // អនុញ្ញាតការទម្លាក់
    }

    function drag(ev) {
      ev.dataTransfer.setData("text", ev.target.id);
    }

    function drop(ev) {
      ev.preventDefault();
      const data = ev.dataTransfer.getData("text");
      ev.target.appendChild(document.getElementById(data));
    }
  </script>

</body>
</html>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. សរសេរកូដ Drag and Drop ខាងលើ រួចសាកល្បងអូស Element ឆ្លាស់គ្នាទៅវិញទៅមកលើ Browser។
2. តើ Tag មួយណាដែលចាំបាច់ត្រូវមាន attribute `draggable="true"`?
