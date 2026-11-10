# 🔴 Crimson Glitch Boot Animation (KernelSU-Next Module)

A systemless Android boot animation module that transforms the stock boot animation into a **Crimson Red Glitch** theme. Built for **KernelSU-Next**, with full backward compatibility for standard **KernelSU**, **Magisk**, and **APatch**.

---

## ✨ Features

* **Crimson Red Palette:** Converts the original cyan/blue animation into a deep crimson red (`#EC0407`) with high-contrast highlights.
* **Dynamic Glitch Effects:** Features horizontal slice displacements, block artifacts, and ghost-echo frames across `part0`, `part1`, and `part2`.
* **Native 60 FPS:** Runs at `1080x1080` resolution at `60 FPS` using optimized 8-bit indexed PNG frames and zero-compression (`ZIP_STORED`) packaging.
* **Smart Path Detection:** Automatically detects and overlays your ROM's active `bootanimation.zip` location during installation:
  * `/system/product/media`
  * `/system/media`
  * `/system/vendor/media`
  * `/system/system_ext/media`
* **100% Systemless:** Modifies nothing on your raw partitions. Disabling or uninstalling the module immediately restores your original boot animation.

---

## 📦 Installation

### Via KernelSU-Next / KernelSU / Magisk / APatch
1. Download the latest `Crimson_Glitch_BootAnimation_KSU_Next_Module.zip` from the **Releases** page.
2. Open your root manager app (**KernelSU-Next**, **KernelSU**, **Magisk**, or **APatch**).
3. Navigate to the **Modules** tab and tap **Install**.
4. Select the downloaded `.zip` file and wait for the installation script to finish.
5. Tap **Reboot** to apply the new boot animation.

---

## 🛠️ Automated GitHub Actions Build

This repository includes a GitHub Actions workflow (`.github/workflows/build-ksu-module.yml`) that automatically processes a base `bootanimation.zip` and packages the flashable module:

1. Place your base `bootanimation.zip` in the root of this repository.
2. Push your changes or trigger the workflow manually under **Actions → Build Crimson Glitch KSU-Next Module → Run workflow**.
3. Download the compiled `Crimson_Glitch_BootAnimation_KSU_Next_Module.zip` from the workflow run's **Artifacts** section.

---

## 🔄 Uninstallation

* Open your root manager app, go to **Modules**, and tap **Uninstall** (or toggle the module off) on **Crimson Glitch Boot Animation**, then reboot.
* If you are in custom recovery (TWRP/OrangeFox), delete `/data/adb/modules/crimson_glitch_bootanim` and reboot.
