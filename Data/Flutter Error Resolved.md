## **Error:** Dart SDK is not configured
**Step 1:** Check Flutter is installed.
 => Run this bottom given command in CMD. 
```bash
flutter doctor
```

**Step 2:** Find Dart SDK path
=> mostly we set this path in flutter SDK. but in your case flutter SDK in different path then follow you your path. 
```bash
C:\flutter\bin\cache\dart-sdk
```

**Step 3:** Set Path Dart Path / Fix in Android Studio
1. Open **Android Studio**
2. Go to **File → Settings**
3. Search **Dart**
4. Enable ✅ **Dart support**
5. Set **Dart SDK path** (bottom given / and you find this path in **Step 2**)
```bash
flutter/bin/cache/dart-sdk
```
6. Enable Dart support for the following modules
7. Apply → OK
8. Restart Android Studio 🔁

