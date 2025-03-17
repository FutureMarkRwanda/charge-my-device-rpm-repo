# Charge My Device RPM Repository

This repository provides the `charge-my-device` RPM package for Fedora, allowing you to install the Charge My Device application, to seamlessly charge your device using PresenceEye Smart Extensions. It automates charging tasks and monitors your device’s power levels, ensuring efficient and reliable power management.

## Installation Instructions

To install `charge-my-device` on Fedora, follow these steps:

1. **Add the repository**:
```bash
sudo curl -o /etc/yum.repos.d/charge-my-device.repo https://raw.githubusercontent.com/FutureMarkRwanda/charge-my-device-rpm-repo/main/charge-my-device.repo
```

2. **Import the GPG key**:
```bash
sudo rpmkeys --import https://raw.githubusercontent.com/FutureMarkRwanda/charge-my-device-rpm-repo/main/RPM-GPG-KEY-charge-my-device
```

3. **Refresh DNF cache**:
```bash
sudo dnf makecache
```

4. **Install Presence Eye**:
```bash
sudo dnf install charge-my-device
```

After installation, you can launch the app from the terminal with `charge_my_device` or find it in your application menu.

## Package Details
- **Name**: charge-my-device
- **Version**: 1.0
- **Release**: 1.fc41
- **Architecture**: x86_64
- **License**: Proprietary
- **Summary**: PresenceEye Smart Extensions Control App

## Changelog
### **Version 1.0 - (March 17, 2025)**
- Initial release.

## Notes
- This repository uses GPG signing for security. The public key is included as `RPM-GPG-KEY-charge-my-device`.
- If upgrading from an older version, run:
  ```bash
  sudo dnf upgrade charge-my-device
  ```

## Maintainer
- HIRWA RUKUNDO Hope <rw.byose@gmail.com>
