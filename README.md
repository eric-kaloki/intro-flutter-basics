# Flutter & Dart Environment Setup

This guide will help you install Flutter (and Dart) on Windows, macOS, and Linux, and walk you through creating and running your first Flutter application.

---

## Table of Contents

- [System Requirements](#system-requirements)
- [Installing Flutter (and Dart)](#installing-flutter-and-dart)
  - [Windows](#windows)
  - [macOS](#macos)
  - [Linux](#linux)
- [Setting Up Your Editor](#setting-up-your-editor)
- [Creating Your First Flutter App](#creating-your-first-flutter-app)
- [Troubleshooting](#troubleshooting)
- [Additional Resources](#additional-resources)

---

## System Requirements

- **Operating Systems:** Windows 7 SP1 or later, macOS (10.14 or later), Linux (64-bit)
- **Tools:** Git, PowerShell (Windows), Terminal (macOS/Linux)
- **Disk Space:** At least 1.64 GB (not including disk space for IDE/tools)

---

## Installing Flutter and Dart

> **Note:** Flutter includes Dart, so installing Flutter will set you up with Dart automatically.

### Windows

1. **Download Flutter SDK:**
   - Visit the [Flutter Windows installation page](https://docs.flutter.dev/get-started/install/windows) and download the latest Flutter SDK ZIP file.

2. **Extract the ZIP:**
   - Extract the ZIP file to a desired location (e.g., `C:\src\flutter`).

3. **Update Your PATH:**
   - Add `C:\src\flutter\bin` to your system's PATH environment variable.
   - [Learn how to update PATH on Windows](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/).

4. **Run Flutter Doctor:**
   - Open PowerShell and run:
     ```bash
     flutter doctor
     ```
   - Follow the instructions to install any missing dependencies.

### macOS

1. **Download Flutter SDK:**
   - Visit the [Flutter macOS installation page](https://docs.flutter.dev/get-started/install/macos) and download the latest Flutter SDK.

2. **Extract the Archive:**
   - Extract the archive to a suitable location (e.g., `~/development/flutter`).

3. **Update Your PATH:**
   - Open your terminal and add the following to your shell profile (e.g., `~/.bashrc` or `~/.zshrc`):
     ```bash
     export PATH="$PATH:`pwd`/flutter/bin"
     ```
   - Restart your terminal.

4. **Run Flutter Doctor:**
   - Run:
     ```bash
     flutter doctor
     ```
   - Follow any additional setup instructions.

### Linux

1. **Download Flutter SDK:**
   - Visit the [Flutter Linux installation page](https://docs.flutter.dev/get-started/install/linux) and download the latest Flutter SDK tarball.

2. **Extract the Tarball:**
   - Extract it to a desired location (e.g., `~/development/flutter`):
     ```bash
     tar xf flutter_linux_v<version>-stable.tar.xz
     ```

3. **Update Your PATH:**
   - Add Flutter to your PATH by updating your shell profile (e.g., `~/.bashrc` or `~/.zshrc`):
     ```bash
     export PATH="$PATH:~/development/flutter/bin"
     ```
   - Reload your profile:
     ```bash
     source ~/.bashrc
     ```

4. **Run Flutter Doctor:**
   - Run:
     ```bash
     flutter doctor
     ```
   - Address any issues reported.

---

## Setting Up Your Editor

- **Visual Studio Code:**
  - Install [VS Code](https://code.visualstudio.com/).
  - Install the **Flutter** and **Dart** extensions from the VS Code marketplace.

- **Android Studio:**
  - Download and install [Android Studio](https://developer.android.com/studio).
  - During setup, ensure the Flutter plugin is installed (this also installs the Dart plugin).

- **IntelliJ IDEA:**
  - Install IntelliJ IDEA and add the Flutter plugin via the plugins marketplace.

---

## Creating Your First Flutter App

1. **Create a New Project:**
   - Open your terminal and run:
     ```bash
     flutter create my_first_app
     ```
   - This command creates a new Flutter project in the `my_first_app` directory.

2. **Navigate to Your Project:**
   ```bash
   cd my_first_app
