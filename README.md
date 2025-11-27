<!doctype html>
<html lang="ar">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>تحميل vCard</title>
  <style>
    body { font-family: system-ui, Arial, sans-serif; padding: 2rem; direction: rtl; }
    .card { max-width: 720px; margin: auto; text-align: center; }
    a.button { display: inline-block; padding: .6rem 1rem; background:#0366d6; color:#fff; text-decoration:none; border-radius:6px; }
  </style>
</head>
<body>
  <main class="card">
    <h1>تحميل ملف vCard</h1>
    <p>اضغط الزر لتحميل ملف vCard الذي يمكن استيراده إلى جهات الاتصال.</p>
    <p><a class="button" href="./my-vcard.vcf" download>تحميل vCard</a></p>
    <p>أو افتح هذا الرابط مباشرة: <br><code id="link"></code></p>
  </main>
  <script>
    document.getElementById('link').textContent = location.origin + location.pathname.replace(/\/[^\/]*$/, '/') + 'my-vcard.vcf';
  </script>
</body>
</html>
