# Flutter iOS Unsigned IPA Builder (via GitHub Actions) 🚀

This repository provides a quick and free solution for **Flutter** developers using **Windows** or **Linux** who want to test their applications on **iOS** devices (iPhone/iPad).

Using this workflow, you can build an `.ipa` file entirely in the cloud—without needing macOS, Xcode, or a paid Apple Developer account—and install it on your device using tools like Sideloadly.

## ✨ Features
- **No Mac Required:** The entire build process runs on GitHub Actions servers.
- **100% Free:** Utilizes GitHub Actions' free tier for cloud builds.
- **Bypasses Code Signing:** Uses the `--no-codesign` flag to skip Apple's digital signing requirements during the build phase.
- **Automated:** Outputs a downloadable Zip file containing the ready-to-install IPA.

## 🛠️ Prerequisites
1. A GitHub account.
2. **Sideloadly** installed on your Windows PC (to install the app on your device).
3. A **Free Apple ID** (to sign the app locally on your device).

## 🚀 How to Use

### Step 1: Add the Workflow File to Your Project
Download the `build-unsigned-ipa.yml` file from this repository and place it in your Flutter project's directory:

```text
.github/workflows/build-unsigned-ipa.yml
```

### Step 2: Run the Workflow on GitHub
1. Commit and push your changes to GitHub.
2. Go to the **Actions** tab in your repository.
3. Select the **Build Unsigned IPA** workflow from the left sidebar.
4. Click the **Run workflow** button.
5. Once the build finishes (takes a few minutes), download the `ios-unsigned-ipa.zip` file from the **Artifacts** section at the bottom of the page. This file contains your `.ipa`.

### Step 3: Install on iPhone with Sideloadly
1. Connect your iPhone to your Windows PC via USB.
2. Open the **Sideloadly** application.
3. Drag and drop the extracted `.ipa` file into Sideloadly.
4. Enter your free Apple ID.
5. Click **Start** to install the app on your device.

### Step 4: Trust the Developer
The first time you open the app, you might get an **Untrusted Developer** error. To fix this:

1. Go to your iPhone Settings: **Settings > General > VPN & Device Management**
2. Tap on your Apple ID email under the "Developer App" section.
3. Tap **Trust "[Your Email]"**.

Your app will now launch successfully!

## 🌟 Support
If this repository and the YAML file helped you test your app easily, please support the project by giving it a ⭐ Star. It helps make this tool more visible to other developers!

`#Flutter #iOS #Programming #GitHubActions #Sideloadly #AppDevelopment #FlutterDev`
