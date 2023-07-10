# MR Portal
XR collaboration between CREW and GLUON.
MR Portal is a template for creating mixed reality portals on Android phones and Vive Focus 3 HMD.

## Requirements
Android phones and Vive Focus 3 both run on Android, we use the same configuration.
This is the configuration that worked for us, some libraries may not be required.
It is best to use reasonably recent phones.

- Unreal Engine 5.1
- Android Studio Flamingo
  - SDK Platforms
    - Android API 34
    - Android 10.0
  - SDK Tools
    - SDK Build Tools
      - 30.0.3
      - 29.0.2
    - NDK (Side-by-side)
      - 25.1
      - 21.1
    - Android SDK Command Line Tools
      - Android SDK Command Line Tools 8.0
    - CMAKE
      - 3.10
    - Android Emulator 32.1
    - Android Emulator Hypervisor Driver 2.0.0
    - Android SDK Platform Tools 34.0.3
- Java Development Kit (JDK) 1.8.0.22
- Visual Studio Community 2022
  - .NET Desktop Development
  - Desktop development with C++
  - Mobile Development with C++
  - Game Development with C++
  - Linux and Embedded development with C++

## Configuration
We have preconfigured the Unreal Project, a couple of extra steps need to be taken:

### Android phone preparation
- Make sure you use a **data** USB 3.x cable.
- Your phone should be in developer mode 
  - Read this guide on how to activate it https://developer.android.com/studio/debug/dev-options
  - The exact method to activate developer mode can differ depending on the brand. To find instructions, try searching for "Activate developer mode \<BRAND NAME>" online 
- The following settings need to be activated: 
  - USB Debugging ON
  - Install via USB ON

### Unreal Engine Android SDK Settings (Optional)

These steps are optional, but are useful to explicitly define which installed toolchain components that are to be used.

In the `Project Settings -> Platforms -> Android SDK` settings page, set the following parameters as shown below as similarly as possible depending on your equivalent components are installed.

![Android SDK Settings](/_img/UE_AndroidSDKSettings.png)