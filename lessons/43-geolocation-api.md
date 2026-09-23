# មេរៀនទី ៤៣៖ Geolocation API (ការទាញយកទីតាំង GPS)

> **HTML5 Geolocation API ត្រូវបានប្រើសម្រាប់ទាញយកទីតាំងភូមិសាស្ត្រ (Latitude & Longitude) របស់អ្នកប្រើប្រាស់ (អាស្រ័យលើការយល់ព្រមអនុញ្ញាត User Permission)។**

---

## ១. គោលការណ៍សុវត្ថិភាពនៃ Geolocation

ដោយសារទីតាំងភូមិសាស្ត្រជាទិន្នន័យឯកជនភាព (Privacy) Browser នឹងបង្ហាញផ្ទាំង **Prompt សួរអ្នកប្រើប្រាស់** ជានិច្ច ថាតើអនុញ្ញាតឱ្យគេហទំព័រដឹងពីទីតាំងដែរឬទេ។ ប្រសិនបើអ្នកប្រើចុច "Block" កូដនឹងមិនអាចទាញយកទីតាំងបានឡើយ។

---

## ២. វិធីសាស្ត្រ `getCurrentPosition()`

```html
<!DOCTYPE html>
<html lang="km">
<head>
  <meta charset="UTF-8">
  <title>HTML5 Geolocation Demo</title>
</head>
<body>

  <h2>ស្វែងរកទីតាំងបច្ចុប្បន្នរបស់អ្នក</h2>
  <button onclick="getLocation()">📍 ចុចមើលទីតាំង</button>
  <p id="locationDisplay">មិនទាន់ដំណើរការ...</p>

  <script>
    const display = document.getElementById('locationDisplay');

    function getLocation() {
      // ត្រួតពិនិត្យមើលថាតើ Browser គាំទ្រ Geolocation ឬអត់
      if (navigator.geolocation) {
        display.innerHTML = 'កំពុងទាញយកទីតាំង...';
        navigator.geolocation.getCurrentPosition(showPosition, showError);
      } else {
        display.innerHTML = 'Browser របស់អ្នកមិនគាំទ្រ Geolocation API ទេ។';
      }
    }

    function showPosition(position) {
      const lat = position.coords.latitude;
      const lon = position.coords.longitude;
      display.innerHTML = `✅ ទីតាំងរបស់អ្នកគឺ៖<br><b>Latitude (រយៈទទឹង):</b> ${lat}<br><b>Longitude (រយៈបណ្តោយ):</b> ${lon}`;
    }

    function showError(error) {
      switch(error.code) {
        case error.PERMISSION_DENIED:
          display.innerHTML = '❌ អ្នកប្រើប្រាស់បានបដិសេធការផ្តល់ទីតាំង (Permission Denied)។';
          break;
        case error.POSITION_UNAVAILABLE:
          display.innerHTML = '❌ មិនអាចទាញយកព័ត៌មានទីតាំងបានទេ។';
          break;
        case error.TIMEOUT:
          display.innerHTML = '❌ ការទាញយកទីតាំងហួសពេលកំណត់ (Timeout)។';
          break;
        default:
          display.innerHTML = '❌ មានកំហុសមិនស្គាល់មួយបានកើតឡើង។';
      }
    }
  </script>

</body>
</html>
```

---

## ✍️ លំហាត់អនុវត្តសម្រាប់សិស្ស (Practice Exercises)

1. សរសេរកូដ HTML + JavaScript ខាងលើ រួចចុច Allow Permission ដើម្បីពិនិត្យមើល Latitude និង Longitude នៃទីតាំងផ្ទាល់របស់អ្នក។
2. សាកល្បងយក Latitude និង Longitude ដែលទទួលបាន ទៅបើកលើ Google Maps (`https://www.google.com/maps?q=LAT,LON`)។
