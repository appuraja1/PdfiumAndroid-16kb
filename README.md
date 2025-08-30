# PdfiumAndroid-16kb

[![JitPack](https://jitpack.io/v/appuraja1/PdfiumAndroid-16kb.svg)](https://jitpack.io/#appuraja1/PdfiumAndroid-16kb)

## 📖 Introduction
This repository is a maintained fork of [barteksc/PdfiumAndroid](https://github.com/barteksc/PdfiumAndroid).  
It adds **support for 16 KB memory page sizes in Android 15** while staying fully compatible with existing PdfiumAndroid integrations.

Google Play now requires all apps targeting **Android 15+** to support **16 KB page sizes** for native libraries.  
This fork ensures that your PDF rendering apps built on Pdfium remain **installable, crash-free, and Play Store compliant**.

---

## 🚀 Key Features
- ✅ **16 KB page size support** for Android 15+
- 🔄 Upgraded to **[PDFium 133.0.6927.0](https://github.com/bblanchon/pdfium-binaries/releases/tag/chromium%2F6927)**
- 📦 Updated **[libpng v1.6.44](https://github.com/pnggroup/libpng/releases/tag/v1.6.44)**
- 🎨 Updated **[FreeType2 v2.10.0](https://download.savannah.gnu.org/releases/freetype/)**
- 🛠️ Includes **CMakeLists.txt** for building Pdfium `.so` libraries
- 🔒 Apache 2.0 licensed — free for commercial & open-source use

---

## 📦 Dependency Setup

Add **JitPack** to your repositories in `settings.gradle`:
```gradle
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        mavenCentral()
        maven { url "https://jitpack.io" }
    }
}

Then add the dependency in your app/build.gradle:

dependencies {
    implementation "com.github.appuraja1:PdfiumAndroid-16kb:v2.4"
}
