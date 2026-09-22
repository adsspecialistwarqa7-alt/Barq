# برق — Landing Page

Landing page لعلامة "برق" (Lightning)، مبنية كملف HTML واحد self-contained (كل الـ CSS والـ JS جواه، عدا مكتبتين بيتحمّلوا من CDN: GSAP وLenis للسكرول السلس).

## المحتوى
- `index.html` — الصفحة كاملة (اللوجو مضمّن جوه الملف كـ base64، مفيش صور خارجية).

## التشغيل محلي
مفيش build step. افتح `index.html` في المتصفح مباشرة، أو شغّل سيرفر بسيط:

```bash
npx serve .
```

## النشر على Vercel
1. اربط الريبو ده بحساب Vercel (Import Project → اختار الريبو).
2. Framework Preset: **Other** (مفيش build command، الـ Output Directory هو الـ root).
3. Deploy.

مفيش أي إعدادات إضافية مطلوبة — الملف static بالكامل.

## ملاحظات
- المحتوى النصي (الخدمات، الأرقام، دراسات الحالة) حالياً placeholder، لازم يتستبدل بمحتوى حقيقي قبل الإطلاق.
- الأنيميشن بيحترم `prefers-reduced-motion` تلقائيًا.
