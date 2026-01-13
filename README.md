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

---

## GitHub Codespaces Free Tier Usage

GitHub Codespaces offers a free tier for personal accounts. Be mindful of the following limits to avoid unexpected charges:

### Free Tier Allowances

| Resource | Monthly Allowance |
|----------|-------------------|
| Core hours | 120 core-hours |
| Storage | 15 GB-months |

### Understanding Core Hours

Core hours are calculated based on the machine type you use:

- **2-core machine**: 1 hour = 2 core-hours (60 free hours/month)
- **4-core machine**: 1 hour = 4 core-hours (30 free hours/month)
- **8-core machine**: 1 hour = 8 core-hours (15 free hours/month)
- **16-core machine**: 1 hour = 16 core-hours (7.5 free hours/month)

### Best Practices to Stay Within Free Tier

1. **Stop your Codespace when not in use** - Click "Stop Codespace" in the Codespace menu or use `Ctrl+Shift+P` → "Codespaces: Stop Current Codespace"

2. **Use the smallest machine type** - A 2-core machine is often sufficient for building Android applications

3. **Set a shorter idle timeout** - By default, Codespaces stop after 30 minutes of inactivity. You can reduce this in your settings

4. **Delete unused Codespaces** - Go to [github.com/codespaces](https://github.com/codespaces) to manage and delete old Codespaces

5. **Monitor your usage** - Check your usage at [github.com/settings/billing](https://github.com/settings/billing)

### Setting a Spending Limit

To prevent unexpected charges, set a spending limit of $0:

1. Go to **Settings** → **Billing and plans** → **Spending limits**
2. Set the Codespaces spending limit to **$0**

This ensures you will never be charged beyond the free tier.

---

### References

For further documentation on the app, please refer to the [CameraAccess README](CameraAccess/README.md)
For details regarding the Meta Wearables Data Access Framework, please refer to the [Meta Wearables Data Access Framework README](https://wearables.developer.meta.com/docs/develop)
