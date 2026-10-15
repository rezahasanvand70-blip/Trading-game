# Trading Game — شبیه‌ساز ترید

بازی اندرویدی فارسی برای تمرین معامله‌گری با سرمایه مجازی؛ شامل نمودار کندلی شبیه‌سازی‌شده، بازارهای طلا، فارکس، نفت، شاخص و بیت‌کوین، خرید و فروش، حد ضرر/حد سود، اعتبار و گزارش معاملات.

> این پروژه آموزشی است. قیمت‌ها ساختگی هستند و داده بازار واقعی یا توصیه سرمایه‌گذاری نیستند. هیچ سفارش واقعی ثبت نمی‌شود.

## اجرای محلی
پروژه با Capacitor 6 بسته‌بندی می‌شود. نیازمندی‌ها: Node.js 20، Java 17 و Android SDK.

```bash
npm install
npx cap add android
npx cap sync android
cd android
./gradlew assembleDebug
```

APK آزمایشی در `android/app/build/outputs/apk/debug/app-debug.apk` ساخته می‌شود.

## ساخت خودکار
GitHub Actions با هر push به شاخه `main` پروژه Android را می‌سازد و APK آزمایشی را به‌عنوان Artifact نگه می‌دارد. به مسیر **Actions → Android APK → Run details → Artifacts** بروید و artifact با نام `trading-game-debug-apk` را دانلود کنید.

## وضعیت نسخه
Prototype اولیه قابل‌بازی؛ شامل معاملات مجازی پایه و ذخیره موقت در حافظه. ذخیره دائمی پیشرفت، سناریوهای داستانی کامل و اعتبارسنجی عمیق محاسباتی در مراحل بعدی توسعه می‌آیند.
