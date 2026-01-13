# meta-wearables-dat-android-dev

## Building the CameraAccess Sample Application

Follow these steps to build and install the CameraAccess sample application.

### Prerequisites

- GitHub account with access to this repository
- GitHub Personal Access Token (classic)
- Android device with USB debugging enabled
- ADB installed on your local machine

### Step 1: Start the Codespace

Open this repository on GitHub and start a new Codespace.

### Step 2: Set Up Authentication

Export your GitHub Personal Access Token:

```bash
export GITHUB_TOKEN=ghp_... # Your personal access token (classic)
```

### Step 3: Navigate to the Sample Project

Change directory to the CameraAccess sample:

```bash
cd meta-wearables-dat-android-dev/meta/meta-wearables-dat-android/samples/CameraAccess
```

### Step 4: Build the Application

Build the debug APK using Gradle:

```bash
./gradlew assembleDebug
```

### Step 5: Install the APK

The APK will be generated at:

```text
build/outputs/apk/debug/app-debug.apk
```

Download the APK to your local machine, then install it on your Android device using ADB:

```bash
adb install app-debug.apk
```
