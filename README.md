# موقع الأدوات المجانية (Free Tools)

موقع أدوات أونلاين مجانية جاهز للنشر على GitHub Pages، مع أماكن مخصصة لإعلانات Adsterra.

## 📁 محتوى المشروع

```
index.html              الصفحة الرئيسية
about.html              صفحة من نحن
privacy.html           سياسة الخصوصية (مطلوبة للموافقة على Adsterra)
css/style.css          تصميم الموقع
js/main.js             سكربت عام
tools/                 صفحات الأدوات (6 أدوات)
robots.txt             لمحركات البحث
sitemap.xml            خريطة الموقع
.nojekyll              مهم لـ GitHub Pages
```

---

## 🚀 خطوة 1: النشر على GitHub Pages (مجاني، 24 ساعة)

1. أنشئ حساباً على https://github.com إن لم يكن لديك.
2. أنشئ مستودعاً (Repository) جديداً، مثلاً باسم `tools`.
3. من مجلد المشروع نفّذ الأوامر (بعد استبدال الرابط):

```bash
git init
git add .
git commit -m "أول نسخة من الموقع"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO.git
git push -u origin main
```

4. في صفحة المستودع على GitHub: **Settings → Pages**.
5. تحت **Source** اختر الفرع `main` والمجلد `/ (root)` ثم **Save**.
6. بعد دقيقة سيصبح موقعك متاحاً على:
   `https://USERNAME.github.io/REPO/`
   (يعمل 24 ساعة مجاناً وبشكل دائم).

> استبدل `USERNAME` و `REPO` باسمك واسم المستودع في ملفات:
> `index.html` (canonical) و `robots.txt` و `sitemap.xml`.

---

## 💰 خطوة 2: التسجيل في Adsterra والحصول على الأكواد

1. سجّل كـ **Publisher** على: https://adsterra.com
2. فعّل حسابك عبر رابط التأكيد في بريدك.
3. من لوحة التحكم: **Websites → Add Website** وأضف رابط موقعك
   (`https://USERNAME.github.io/REPO/`).
4. انتظر الموافقة (عادة سريعة لمواقع بها محتوى + صفحة خصوصية — وهي جاهزة عندك).
5. بعد الموافقة: **Websites → Ad Units → Create** واختر نوع الإعلان:
   - **Banner** (مثل 728x90 أو 300x250) — للمساحات في الصفحات.
   - **Social Bar** — شريط سفلي عائم (أرباح جيدة).
   - **Popunder** — نافذة خلفية (أعلى ربح لكن أقل تجربة مستخدم).
   - **Native Banner** — إعلان يشبه المحتوى.
6. انسخ كود كل وحدة إعلانية (JavaScript snippet).

## 🧩 خطوة 3: لصق أكواد Adsterra في الموقع

في كل صفحة ستجد أماكن الإعلانات مكتوبة هكذا:

```html
<div class="ad-slot container"><span class="ad-label">مساحة إعلانية</span></div>
```

استبدل السطر بالكامل بكود Adsterra، مثال:

```html
<div class="ad-slot container">
  <script type="text/javascript">
    atOptions = { 'key': 'YOUR_KEY', 'format':'iframe', 'height':90, 'width':728, 'params':{} };
  </script>
  <script src="//www.highperformanceformat.com/YOUR_KEY/invoke.js"></script>
</div>
```

أما إعلانات **Social Bar / Popunder** فتُلصق مرة واحدة قبل `</head>` أو قبل `</body>`
في ملف `index.html` وباقي الصفحات.

بعد التعديل، احفظ الملفات وأعد الرفع:

```bash
git add .
git commit -m "إضافة أكواد Adsterra"
git push
```

---

## 📈 خطوة 4: جلب الزيارات وزيادة الأرباح

- **SEO**: أضف موقعك في [Google Search Console](https://search.google.com/search-console)
  وأرسل ملف `sitemap.xml`.
- **محتوى**: أضف أدوات ومقالات جديدة باستمرار (كل أداة = صفحة تجلب زيارات).
- **السوشيال ميديا**: شارك الأدوات في فيسبوك، تويتر، تيك توك، مجموعات وبنترست.
- **الكلمات المفتاحية**: استهدف عبارات يبحث عنها الناس مثل "مولد كلمات مرور".
- **السرعة**: الموقع خفيف وسريع = ترتيب أفضل في جوجل.
- **ملاحظة مهمة**: لا تضغط على إعلاناتك بنفسك ولا تستخدم زيارات وهمية (Bots)،
  لأن Adsterra يوقف الحسابات المخالفة.

---

## ⚠️ ملاحظات

- استبدل `your-email@example.com` في `about.html` ببريدك.
- Adsterra لا يتطلب `ads.txt` غالباً، لكن إن طلبه ضعه في الجذر.
- الحد الأدنى للسحب من Adsterra يبدأ من 5$ (حسب طريقة الدفع).
