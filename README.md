# EduFeeMaker Android App 📱
## School Fee Management WebView App

### 🌐 Website: https://edufeemaker.page.gd

---

## ✅ Features Included

| Feature | Status |
|---|---|
| Splash Screen with Animation | ✅ |
| Custom App Icon (Education Logo) | ✅ |
| WebView with Full Screen | ✅ |
| Bottom Navigation Auto-Hide (JS Inject) | ✅ |
| Top Progress Bar (Loading) | ✅ |
| Double-Back Button to Exit | ✅ |
| File Upload Support | ✅ |
| Camera Capture Support | ✅ |
| Download Manager | ✅ |
| Pull to Refresh (SwipeRefresh) | ✅ |
| Internet Connection Check | ✅ |
| No Internet Page (Bangla) | ✅ |
| Full Screen Mode | ✅ |
| Release APK & AAB Ready | ✅ |
| FileProvider (Android 7+) | ✅ |
| Network Security Config | ✅ |

---

## 🚀 Android Studio Setup Steps

### Step 1: Open Project
1. Android Studio খুলুন → **"Open an Existing Project"**
2. এই `EduFeeMaker` ফোল্ডারটি সিলেক্ট করুন
3. Gradle Sync হওয়ার জন্য অপেক্ষা করুন

### Step 2: Minimum Requirements
- **Android Studio:** Hedgehog (2023.1.1) বা নতুন
- **JDK:** 17
- **Gradle:** 8.2
- **compileSdk:** 34
- **minSdk:** 21 (Android 5.0+)

### Step 3: Build Debug APK
```
Build → Build Bundle(s)/APK(s) → Build APK(s)
```
APK পাবেন: `app/build/outputs/apk/debug/app-debug.apk`

### Step 4: Build Release AAB (Play Store)
1. `Build → Generate Signed Bundle / APK`
2. **Android App Bundle** সিলেক্ট করুন
3. Keystore তৈরি করুন (প্রথমবার হলে **Create New...**)
4. Build করুন → `app/build/outputs/bundle/release/app-release.aab`

---

## 🎨 Customize করতে চাইলে

### রং পরিবর্তন:
`app/src/main/res/values/colors.xml`
```xml
<color name="colorPrimary">#1565C0</color>   <!-- Main blue color -->
<color name="colorAccent">#FFC107</color>    <!-- Gold accent -->
<color name="splash_bg">#1565C0</color>      <!-- Splash background -->
```

### URL পরিবর্তন:
`MainActivity.java` এ:
```java
private static final String APP_URL = "https://edufeemaker.page.gd";
```

### Splash Duration পরিবর্তন:
`SplashActivity.java` এ:
```java
private static final int SPLASH_DURATION = 2500; // milliseconds
```

### App Name পরিবর্তন:
`app/src/main/res/values/strings.xml`
```xml
<string name="app_name">EduFeeMaker</string>
```

---

## 📦 Play Store Checklist

- [ ] Keystore দিয়ে Sign করুন
- [ ] `versionCode` ও `versionName` আপডেট করুন (`app/build.gradle`)
- [ ] App Icon PNG ফরম্যাটে দিন (512x512)
- [ ] Screenshots তৈরি করুন
- [ ] Privacy Policy URL যোগ করুন
- [ ] AAB ফাইল Upload করুন (APK নয়)

---

## 📁 Project Structure

```
EduFeeMaker/
├── app/
│   ├── src/main/
│   │   ├── java/com/edufeemaker/app/
│   │   │   ├── SplashActivity.java      ← Splash Screen
│   │   │   └── MainActivity.java        ← Main WebView
│   │   ├── res/
│   │   │   ├── layout/
│   │   │   │   ├── activity_splash.xml  ← Splash Layout
│   │   │   │   └── activity_main.xml    ← Main Layout
│   │   │   ├── drawable/
│   │   │   │   ├── ic_logo.xml          ← App Logo
│   │   │   │   └── ic_no_internet.xml   ← No Internet Icon
│   │   │   ├── values/
│   │   │   │   ├── colors.xml
│   │   │   │   ├── strings.xml
│   │   │   │   └── themes.xml
│   │   │   └── xml/
│   │   │       ├── network_security_config.xml
│   │   │       └── file_paths.xml
│   │   └── AndroidManifest.xml
│   └── build.gradle
├── build.gradle
├── settings.gradle
└── README.md
```

---

**Made with ❤️ for EduFeeMaker**
