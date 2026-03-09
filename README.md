# 📱 Calculator App — Build Instructions

## What's Inside
A clean, dark-themed Android calculator app with:
- Addition, Subtraction, Multiplication, Division
- Decimal support, sign toggle (+/-), backspace
- Expression history display
- Supports Android 5.0+ (API 21+)

---

## ✅ Step-by-Step: Build the APK

### Step 1 — Install Android Studio
Download from: https://developer.android.com/studio
(Free, available for Windows, Mac, Linux)

### Step 2 — Open the Project
1. Launch Android Studio
2. Click **"Open"** (not "New Project")
3. Navigate to and select the **CalculatorApp** folder
4. Wait for Gradle sync to complete (~2-5 minutes first time)

### Step 3 — Build the APK
Go to the menu bar:
```
Build → Build Bundle(s) / APK(s) → Build APK(s)
```

### Step 4 — Find Your APK
When build finishes, a notification will appear at the bottom.
Click **"locate"** in the notification, OR find it at:
```
CalculatorApp/app/build/outputs/apk/debug/app-debug.apk
```

### Step 5 — Install on Your Phone
**Option A — USB:**
1. Enable Developer Options on your phone
   (Settings → About Phone → tap "Build Number" 7 times)
2. Enable "USB Debugging"
3. Connect phone via USB
4. In Android Studio click the ▶ Run button

**Option B — File Transfer:**
1. Copy `app-debug.apk` to your phone
2. On your phone, open the APK file
3. Allow "Install from unknown sources" if prompted
4. Tap Install

---

## Project Structure
```
CalculatorApp/
├── app/
│   └── src/main/
│       ├── java/com/example/calculator/
│       │   └── MainActivity.kt          ← All calculator logic
│       ├── res/
│       │   ├── layout/activity_main.xml ← UI layout
│       │   ├── drawable/                ← Button styles
│       │   └── values/                  ← Colors, strings, theme
│       └── AndroidManifest.xml
├── build.gradle
└── settings.gradle
```

---

## Troubleshooting
- **Gradle sync fails?** → Check internet connection (first sync downloads dependencies)
- **"SDK not found"?** → Android Studio will prompt you to install SDK — click Install
- **Build errors?** → Go to File → Invalidate Caches → Restart
