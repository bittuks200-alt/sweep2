SweepSignals - Android (Kotlin + Jetpack Compose)

1. Install Android Studio (Koala or newer).
2. File > Open > select this SweepSignals folder. Let Gradle sync (needs internet; it downloads Gradle 8.7).
3. Connect phone (USB debugging ON) or use emulator, press Run.
4. Allow notifications. Tap "Start monitoring".
   Xiaomi/Redmi: Settings > Apps > Sweep Signals > Battery saver > "No restrictions", and enable Autostart,
   otherwise MIUI kills the background service.
5. To get an APK to share: Build > Build Bundle(s)/APK(s) > Build APK(s).

Tuning: see Config in Strategy.kt (swingLookback, signalExpiry, readyExpiry, oneTradePerDay).

NO ANDROID STUDIO? Build online with GitHub Actions:
1. Make a free GitHub account, create a new repository.
2. Upload ALL files of this folder (including the hidden .github folder) to the repo.
3. Open the Actions tab > "Build APK" > wait ~5 min until green.
4. Open that run > Artifacts > download SweepSignals-apk > unzip > install app-debug.apk on the phone.
