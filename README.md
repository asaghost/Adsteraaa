# موقع الأدوات المجانية (Free Tools) — ملف واحد

موقع أدوات أونلاين مجانية ضخم (أكثر من 40 أداة) في **ملف HTML واحد** جاهز للنشر على GitHub Pages، مع أماكن مخصصة لإعلانات Adsterra.

## ✨ الأدوات (مقسّمة لفئات)

- **📝 النصوص**: عداد الكلمات، محول الحالة، عكس النص، إزالة المكرر، فرز الأسطر، نص Lorem، تنسيق جمالي، مقارنة نصين.
- **🖼️ الصور**: تغيير الحجم، ضغط، تحويل الصيغة، علامة مائية، تدوير/قلب.
- **📄 PDF**: دمج، تقسيم (نطاق صفحات)، صور→PDF، تدوير الصفحات، معلومات الملف، PDF→صور.
- **💻 المطورين**: تنسيق JSON، Base64، ترميز URL، UUID، الطابع الزمني، هاش SHA-256، HTML Escape.
- **🧮 الحسابات**: العمر، محول الوحدات، BMI، النسبة المئوية، القرض، آلة حاسبة.
- **⏰ التاريخ والوقت**: العد التنازلي، ساعة العالم، الفرق بين تاريخين.
- **🎨 الألوان**: محول HEX/RGB/HSL، منتقي الألوان.
- **✨ متنوع**: رمز QR، باركود، مولد كلمات المرور، فاحص القوة، أرقام عشوائية، أسماء مستخدمين.

> المكتبات من CDN: pdf-lib، pdf.js، JsBarcode، JSZip. تحتاج اتصال إنترنت لبعض الأدوات.

---

## 🚀 النشر على GitHub Pages (مجاني، يعمل 24 ساعة)

1. أنشئ مستودعاً على https://github.com (مثلاً `tools`).
2. من مجلد المشروع:
```bash
git init
git add .
git commit -m "موقع الأدوات"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO.git
git push -u origin main
```
3. **Settings → Pages** ← اختر `main` و `/ (root)` ثم Save.
4. الموقع يصبح على `https://USERNAME.github.io/REPO/`.

> استبدل `USERNAME` و `REPO` في: `index.html` (canonical)، `robots.txt`، `sitemap.xml`.

---

## 💰 إعلانات Adsterra

1. سجّل كـ Publisher على https://adsterra.com وأضف رابط موقعك.
2. بعد الموافقة أنشئ Ad Units (Banner / Social Bar / Popunder / Native).
3. في `index.html` استبدل `<div class="ad-slot ...">` بالكود، مثال:
```html
<div class="ad-slot container">
  <script type="text/javascript">
    atOptions = { 'key':'YOUR_KEY','format':'iframe','height':90,'width':728,'params':{} };
  </script>
  <script src="//www.highperformanceformat.com/YOUR_KEY/invoke.js"></script>
</div>
```
4. Social Bar/Popunder تُلصق مرة واحدة قبل `</head>` أو قبل `</body>`.

---

## 📈 جلب الزيارات والأرباح

- أرسل `sitemap.xml` في Google Search Console.
- شارك الأدوات على السوشيال ميديا والمجموعات.
- أضف أدوات/مقالات جديدة باستمرار.
- ⚠️ لا تنقر على إعلاناتك بنفسك ولا تستخدم زيارات وهمية (Adsterra يحظر المخالفين).
