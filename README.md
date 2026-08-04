# Android App – Bluetooth Mouse Bridge

## Requirements

- Android Studio Hedgehog or newer (or any version that supports AGP 8.2)
- Android device / emulator with **API 26+** (Android 8.0 Oreo or higher)
- Bluetooth mouse already paired with the phone

## How to build

1. Open **Android Studio**
2. **File → Open** and select the `android` folder
3. Wait for Gradle sync to finish
4. Connect your phone (USB debugging on) **or** use an emulator
5. Click **Run** (green play button)

The APK will also be generated at:

```
app/build/outputs/apk/debug/app-debug.apk
```

You can copy that file to any phone and install it.

## First use

1. Pair your Bluetooth mouse with the phone (Settings → Bluetooth)
2. Start the **PC server** first (`python mouse_server.py`)
3. Open the app on the phone
4. Type the PC’s local IP address (e.g. `192.168.1.42`)
5. Tap **Connect**
6. Tap the large dark area once → pointer capture starts
7. Move the Bluetooth mouse → the PC cursor moves

You can also use your finger on the dark area as a trackpad.

Left / Right buttons at the bottom work even without the physical mouse.
