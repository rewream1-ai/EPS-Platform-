# 🏆 EPS Platform — منصة التربية البدنية والرياضية

<div align="center">
  <img src="icons/icon-192x192.png" width="120" alt="EPS Platform Logo"/>
  <h3>منصة إدارية شاملة لأستاذ التربية البدنية والرياضية</h3>
  <p>
    <a href="https://YOUR_USERNAME.github.io/eps-platform"><strong>🌐 فتح التطبيق</strong></a> ·
    <a href="#-تحميل-تطبيق-سطح-المكتب">💻 تطبيق سطح المكتب</a> ·
    <a href="#-تطبيق-أندرويد">📱 تطبيق أندرويد</a>
  </p>
</div>

---

## ✨ الميزات

- 📊 **لوحة تحكم** — إحصائيات وتقارير فورية
- 👥 **إدارة المتعلمين** — بيانات شاملة لكل تلميذ
- 📝 **التقييمات** — تسجيل درجات التربية البدنية
- 🔥 **Firebase** — مزامنة البيانات السحابية (اختياري)
- 🌙 **وضع ليلي / نهاري**
- 📲 **PWA** — قابل للتثبيت كتطبيق مستقل
- 🖥️ **Electron** — تطبيق سطح المكتب (Windows / Mac / Linux)
- 📱 **Capacitor** — تطبيق Android

---

## 🚀 استخدام مباشر (GitHub Pages)

بمجرد رفع المشروع على GitHub وتفعيل **GitHub Pages**، ستحصل على رابط مثل:

```
https://YOUR_USERNAME.github.io/eps-platform
```

### خطوات تفعيل GitHub Pages:
1. اذهب إلى **Settings** في المستودع
2. انقر على **Pages** في القائمة اليسرى
3. اختر **Source: GitHub Actions**
4. احفظ — سيتم النشر تلقائياً ✅

---

## 💻 تحميل تطبيق سطح المكتب

### الطريقة السريعة (مع Electron)

```bash
# 1. نسخ المستودع
git clone https://github.com/YOUR_USERNAME/eps-platform.git
cd eps-platform

# 2. تثبيت المتطلبات
npm install

# 3. تشغيل مباشر
npm start

# 4. بناء الملف التنفيذي
npm run build:win    # Windows (.exe)
npm run build:mac    # macOS (.dmg)
npm run build:linux  # Linux (.AppImage)
```

الملف التنفيذي سيكون في مجلد `dist-electron/`

---

## 📱 تطبيق أندرويد

### المتطلبات:
- Node.js 18+
- Android Studio
- JDK 17

### الخطوات:

```bash
# 1. تثبيت المتطلبات
npm install

# 2. إضافة منصة Android
npm run cap:android
# أو يدوياً:
npx cap add android
npx cap sync

# 3. فتح Android Studio
npm run cap:open-android
# أو:
npx cap open android

# 4. بناء APK من Android Studio:
# Build → Generate Signed Bundle/APK → APK
```

> 💡 **ملاحظة:** تأكد من تثبيت Android Studio و JDK 17 قبل البدء.

---

## 📂 هيكل المشروع

```
eps-platform/
├── index.html              # التطبيق الرئيسي (كل شيء في ملف واحد)
├── manifest.json           # إعدادات PWA
├── sw.js                   # Service Worker (العمل بدون إنترنت)
├── capacitor.config.json   # إعدادات Android
├── package.json            # إعدادات Node.js / Electron
├── icons/                  # أيقونات بجميع الأحجام
│   ├── icon-72x72.png
│   ├── icon-192x192.png
│   ├── icon-512x512.png
│   └── icon-256x256.ico    # لـ Windows
├── electron/
│   ├── main.js             # نقطة دخول Electron
│   └── preload.js          # Preload script
└── .github/
    └── workflows/
        ├── deploy-pages.yml   # نشر تلقائي على GitHub Pages
        └── build-electron.yml # بناء تلقائي للتطبيق
```

---

## 🔧 الإعدادات المطلوبة

### Firebase (اختياري)
إذا أردت مزامنة البيانات سحابياً:
1. اذهب إلى [Firebase Console](https://console.firebase.google.com)
2. أنشئ مشروعاً جديداً
3. افتح التطبيق → الإعدادات → أدخل بيانات Firebase

---

## 📋 المتطلبات

| الأداة | الإصدار |
|--------|---------|
| Node.js | 18+ |
| npm | 8+ |
| Electron | 29+ |
| Android Studio | Hedgehog+ (لـ Android) |

---

## 📄 الترخيص

MIT License — للاستخدام الشخصي والتعليمي بحرية.

---

<div align="center">
  <p>صُنع بـ ❤️ من أجل أساتذة التربية البدنية والرياضية</p>
</div>
