# Sharpa Avatar SDK

Sharpa Avatar SDK provides libraries and APIs for integrating Sharpa AvatarExo Glove into custom applications and robotics software stacks.

---

## 📥 Download

Download the latest SDK package from [Releases](https://github.com/sharpa-robotics/sharpa-avatar-sdk/releases).

Choose the package that matches your system architecture:

```
avatar-sdk_<version>_<arch>.deb
```

---

## 🚀 Installation (Ubuntu / Debian)

Install the downloaded package with APT:

```bash
sudo apt install ./avatar-sdk_<version>_<arch>.deb
```

Using `apt install` is recommended because it resolves the SDK's system dependencies automatically.

The SDK is installed under:

```
/opt/avatar-sdk/
```

---

## 📦 Installed layout

| Item | Path |
|---|---|
| C++ headers | `/opt/avatar-sdk/include/` |
| Shared libraries | `/opt/avatar-sdk/lib/` |
| Backend runtime | `/opt/avatar-sdk/bin/avatar-backend` |
| Configuration and resources | `/opt/avatar-sdk/share/` |
| Backend command | `/usr/local/bin/avatar-backend` |

The exact contents and supported Python versions may differ by release and architecture. Check the release notes before installing.

---

## ▶️ Quick check

After installation:

```bash
avatar-backend --help
```

For C++ and Python integration details, use the documentation included with the selected release.

---

## 📱 Sharpa Avatar App

[Sharpa Avatar App](https://github.com/sharpa-robotics/sharpa-avatar-app) and Sharpa Avatar SDK are versioned and released separately.

The supported App installer configures the Sharpa software repository and installs an SDK version compatible with the App. The App package does not contain the SDK; it declares a minimum SDK requirement and APT resolves an available version that satisfies it.

If you are installing the SDK for use with Sharpa Avatar App, follow the App repository's installation instructions instead of installing arbitrary SDK versions manually.

---

## 🔗 Compatibility

| Avatar SDK | Avatar App | Bundled firmware | Notes |
|---|---|---|---|
| 1.7.4 | 1.1.39 | 2.0.7 | Production release |

This table will be updated with every public SDK release.

---

## 🔄 Update

Install the newer package with APT:

```bash
sudo apt install ./avatar-sdk_<new-version>_<arch>.deb
```

When the SDK is managed as an App dependency, use the matching Sharpa Avatar App installer bundle for the supported upgrade path.

---

## ❌ Uninstall

For a standalone SDK installation:

```bash
sudo apt remove avatar-sdk
```

If Sharpa Avatar App is installed, its package dependency may require the SDK to remain installed. Remove or update the App first.

---

## ⚠️ Requirements

- Ubuntu or Debian-based Linux
- x86_64 (amd64) or ARM64, when an asset for that architecture is provided
- C++17 or later for C++ integrations
- A Python version and architecture matching one of the Python modules included in the selected release

---

## Related downloads

- [Sharpa Avatar App](https://github.com/sharpa-robotics/sharpa-avatar-app)
- [Sharpa Avatar Firmware](https://github.com/sharpa-robotics/sharpa-avatar-ae01-firmware)

---

## 📞 Support

For product support, contact [support@sharpa.com](mailto:support@sharpa.com).
