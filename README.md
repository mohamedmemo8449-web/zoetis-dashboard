# نشر داشبورد Zoetis على GitHub Pages

المجلد ده مخصص لمستودع GitHub عام يحتوي على نسخة الداشبورد فقط. ملفات Numbers والمصادر وملفات CSV الأصلية تظل خارج المستودع.

## تحديث الداشبورد

بعد تعديل `../Dashboard_Mohamed_Sales.html`، افتح Terminal من هذا المجلد وشغّل:

```sh
cp ../Dashboard_Mohamed_Sales.html index.html
git add index.html
git commit -m "Update dashboard"
git push
```

كل `git push` إلى فرع `main` ينشر النسخة الجديدة تلقائيًا. يمكن فتح الرابط المنشور على الآيفون وحفظه في الشاشة الرئيسية من Safari.

## إعداد أول مرة

1. أنشئ مستودع GitHub عامًا باسم `zoetis-dashboard`، من غير README أو ملفات إضافية.
2. هذا المجلد مجهز بالفعل كمستودع محلي وفيه أول commit. من Terminal داخله، اربطه بالمستودع البعيد وارفعه:

   ```sh
   git remote add origin https://github.com/mohamedmemo8449-web/zoetis-dashboard.git
   git push -u origin main
   ```

3. من إعدادات المستودع، افتح **Settings → Pages** واختر **GitHub Actions** كمصدر للنشر.
4. انتظر اكتمال **Actions → Publish dashboard**؛ سيظهر رابط الموقع في **Settings → Pages**.

رابط GitHub Pages عام لمن لديه الرابط، كما أن ملفات المستودع متاحة للعامة. لا ترفع إليه ملفات المشروع الأخرى.
