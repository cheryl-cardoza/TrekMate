# Trekking (Android)

An Android 9+ app with a splash screen, login (default: cheryl / 123), registration and forgot-password dialogs, and a simple main screen about trekking.

## Open and Run
1. Open Android Studio Flamingo or newer.
2. File > Open > select the `Trekking` folder.
3. Let Gradle sync. If prompted, install/upgrade the Gradle wrapper and Android Gradle Plugin.
4. Create/select an Android 9 (API 28) or newer emulator.
5. Click Run.

## Features
- Splash screen with logo and loading for 3 seconds.
- Login page with default credentials and SharedPreferences for registered users.
- Registration dialog collects name, age, location, phone, username, password, confirm password.
- Forgot password dialog retrieves stored password for a username.
- Main screen shows basic trekking content.

## Modules
- `app/src/main/java/com/example/trekking/ui/`
  - `SplashActivity.kt`: shows splash then navigates to login.
  - `LoginActivity.kt`: handles login, opens dialogs.
  - `RegistrationDialogFragment.kt`: registers and stores users.
  - `ForgotPasswordDialogFragment.kt`: retrieves password.
  - `MainActivity.kt`: trekking info screen.

## Notes
- Min SDK 28, Target/Compile 34.
- Uses Material components and AppCompat.
- All data is local and non-persistent beyond app storage; no networking.
