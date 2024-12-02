# 🌟 Electrum-Doge: Lightweight Dogecoin Wallet

[![License](https://img.shields.io/github/license/Electrum-doge/electrum-doge)](https://github.com/Electrum-doge/electrum-doge/blob/master/LICENSE)
[![Release](https://img.shields.io/github/v/release/Electrum-doge/electrum-doge)](https://github.com/Electrum-doge/electrum-doge/releases)

**Electrum-Doge** is a secure, lightweight, and efficient wallet for managing your Dogecoin assets. Built on the trusted Electrum framework, it provides fast transactions without downloading the full blockchain. Perfect for Dogecoin enthusiasts who prioritize speed and security.

---

## ✨ Features

- 🚀 **Lightweight**: No need to download the full blockchain.
- 🔒 **Secure Storage**: Your private keys are stored locally and encrypted.
- 🛡 **Hardware Wallet Support**: Compatible with Ledger and Trezor.
- 👥 **Multisignature Support**: Increased security with multiple signatures.
- 💻 **Cross-Platform**: Works on Windows, macOS, and Linux.
- 🥶 **Cold Wallet Functionality**: Ideal for offline Dogecoin storage.

---

## 🛠️ Downloads

Get the latest version of Electrum-Doge for your operating system from the [Releases](https://github.com/Electrum-doge/electrum-doge/releases) page:

- **Windows**: [Download for Windows](https://github.com/Electrum-doge/electrum-doge/releases/download/v.4.1.5/electrum-dogecoin-win10-setup.exe)
- **Linux**: [Download for Linux](https://github.com/Electrum-doge/electrum-doge/releases/download/v.4.1.5/AppImage-electrum-dogecoin-QRFIX-01-03-2022.x86_64)
- **macOS**: [Download for macOS](https://github.com/Electrum-doge/electrum-doge/releases/download/v.4.1.5/electrum-dogecoin-macOS-01-03-2022.dmg)

---

## 📦 Installation

### Running Electrum-Doge Directly

To run Electrum-Doge from the current directory, execute:

```bash
./electrum-doge
```

### Installing Electrum-Doge System-Wide

If you prefer to install Electrum-Doge on your system, allowing you to run it from any directory:

```bash
sudo python setup.py install
electrum-doge
```

---

## 🏗️ Building Official Packages

Follow these steps to create official Electrum-Doge packages.

### General Build Steps

1. **Generate Internationalization Files:**

    ```bash
    python mki18n.py
    ```

2. **Compile Resource Files:**

    ```bash
    pyrcc4 icons.qrc -o gui/qt/icons_rc.py
    ```

3. **Create Source Distribution:**

    ```bash
    python setup.py sdist --format=zip,gztar
    ```

### Building for macOS

#### Using Port-Based Installations

```bash
sudo python setup-release.py py2app
```

#### Using Homebrew Installations

```bash
ARCHFLAGS="-arch i386 -arch x86_64" sudo python setup-release.py py2app --includes sip
```

4. **Create DMG File:**

    ```bash
    sudo hdiutil create -fs HFS+ -volname "Electrum-Doge" -srcfolder dist/Electrum-Doge.app dist/electrum-doge-VERSION-macosx.dmg
    ```

---

## 📖 Documentation

Comprehensive setup instructions, FAQs, and usage guides are available in the [Documentation](https://github.com/Electrum-doge/electrum-doge/tree/master/docs) section of the repository.

---

## 📜 License

This project is licensed under the [GNU GPL v3](https://github.com/Electrum-doge/electrum-doge/blob/master/LICENCE).

---

## 📈 Keywords

Electrum dogecoin, Dogecoin Wallet, Lightweight Wallet, Secure Dogecoin Wallet, Electrum Fork, Multisig Wallet, Dogecoin Blockchain

---

## 👥 Authors

Developed by the Electrum-Doge contributors.

## 🖥️ Language

Written in Python.
