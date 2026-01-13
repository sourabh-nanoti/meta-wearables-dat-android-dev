# meta-wearables-dat-android-dev

## Building the CameraAccess Sample Application

Follow these steps to build and install the CameraAccess sample application.

### Prerequisites

- GitHub account with access to this repository
- GitHub Personal Access Token (classic)
- Android device with USB debugging enabled
- ADB installed on your local machine

### Step 1: Start the Codespace

Open this repository on GitHub and start a new Codespace. You can do this by clicking the "Code" button and selecting "Create Codespace on main".

### Step 2: Set Up Authentication

Once the Codespace is started, go to the Codespace terminal on your browser window and export your GitHub Personal Access Token:

```bash
export GITHUB_TOKEN=ghp_... # Your personal access token (classic)
```

### Step 3: Navigate to the Sample Project

On Codespaces, change directory to the CameraAccess sample:

```bash
cd meta-wearables-dat-android-dev/meta/meta-wearables-dat-android/samples/CameraAccess
```

### Step 4: Build the Application

On Codespaces, build the debug APK using Gradle:

```bash
./gradlew assembleDebug
```

### Step 5: Install the APK

The APK will be generated at:

```text
build/outputs/apk/debug/app-debug.apk
```

Download the APK from Codespaces to your local machine, then install it on your Android device using ADB:

```bash
adb install app-debug.apk
```

### References

For further documentation on the app, please refer to the [CameraAccess README](CameraAccess/README.md)
For details regarding the Meta Wearables Data Access Framework, please refer to the [Meta Wearables Data Access Framework README](https://wearables.developer.meta.com/docs/develop)
