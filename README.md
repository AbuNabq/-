<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ترجملي</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>ترجملي</h1>
        <p>منصة ترجمة تدعم العديد من اللغات الأجنبية واللغة العربية</p>

        <div class="form-group">
            <label for="from-language">من اللغة:</label>
            <select id="from-language">
                <option value="ar">العربية</option>
                <option value="en">الإنجليزية</option>
                <option value="fr">الفرنسية</option>
                <option value="es">الإسبانية</option>
                <option value="de">الألمانية</option>
                <!-- يمكنك إضافة لغات أخرى -->
            </select>
        </div>

        <div class="form-group">
            <label for="to-language">إلى اللغة:</label>
            <select id="to-language">
                <option value="en">الإنجليزية</option>
                <option value="ar">العربية</option>
                <option value="fr">الفرنسية</option>
                <option value="es">الإسبانية</option>
                <option value="de">الألمانية</option>
            </select>
        </div>

        <div class="form-group">
            <label for="input-text">النص المراد ترجمته:</label>
            <textarea id="input-text" rows="5" placeholder="اكتب هنا..."></textarea>
        </div>

        <button onclick="translateText()">ترجمة</button>

        <div class="form-group">
            <label for="output-text">الترجمة:</label>
            <textarea id="output-text" rows="5" readonly></textarea>
        </div>
    </div>

    <script>
        function translateText() {
            // هذا مثال وهمي – يجب ربطه لاحقًا بـ API للترجمة
            const input = document.getElementById("input-text").value;
            const output = document.getElementById("output-text");
            output.value = "الترجمة تظهر هنا (تجريبية)";
        }
    </script>
</body>
</html>
