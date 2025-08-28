# ⚡🧙‍♂️ Wizard's NBD Mounting Suite 🧙‍♀️⚡

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![GitHub issues](https://img.shields.io/github/issues/LINUX-OASIS/NBD-MOUNT-VDI-QCOW)](https://github.com/LINUX-OASIS/NBD-MOUNT-VDI-QCOW/issues)
[![GitHub forks](https://img.shields.io/github/forks/LINUX-OASIS/NBD-MOUNT-VDI-QCOW)](https://github.com/LINUX-OASIS/NBD-MOUNT-VDI-QCOW/network)
[![GitHub stars](https://img.shields.io/github/stars/LINUX-OASIS/NBD-MOUNT-VDI-QCOW)](https://github.com/LINUX-OASIS/NBD-MOUNT-VDI-QCOW/stargazers)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

<p align="center">
  <img src="https://raw.githubusercontent.com/LINUX-OASIS/NBD-MOUNT-VDI-QCOW/main/.github/wizard.png" alt="Wizard ASCII Art" width="200"/>
</p>

An interactive TUI script for easily mounting and unmounting QCOW2 and VDI virtual disk images using Network Block Devices (NBD) on Debian-based systems. Summon devices from the void like a true Discomancer!

---

## ✨ About The Project

This script provides a user-friendly `whiptail` terminal interface to simplify the process of using `qemu-nbd`. Instead of wrestling with complex commands, you can navigate through simple menus to:

- Connect a `.vdi` or `.qcow2` virtual disk image to an available `/dev/nbd*` device.
- Safely unmount all partitions on an NBD device.
- Disconnect the image from the NBD device.

It's designed to be intuitive, safe, and a little bit magical.

### 🔮 Features

*   **Interactive TUI:** Easy-to-use terminal menus powered by `whiptail`.
*   **Mount `.vdi` & `.qcow2`:** Supports the most common virtual disk formats.
*   **Auto-Dependency Check:** Automatically checks for `qemu-utils` and offers to install it.
*   **Smart Device Listing:** Shows which NBD slots are available and which are in use.
*   **Local Image Discovery:** Automatically finds compatible disk images in the current directory for quick selection.
*   **Safe Unmounting:** Intelligently finds and unmounts all filesystems on a device's partitions before disconnecting.
*   **Themed Interface:** A fun "Discomancer" wizard theme with ASCII art and emojis! 🧙

## 🚀 Getting Started

Follow these simple steps to get the script up and running.

### 📋 Prerequisites

The script requires the following packages. Don't worry, it will try to install the main dependency for you!

*   `qemu-utils`: Provides the `qemu-nbd` command. The script will attempt to install this using `apt` if it's missing.
*   `whiptail`: Used for the dialog boxes. This is typically included in most base installations of Debian/Ubuntu.

### ⚙️ Installation

1.  Clone the repository:
    ```sh
    git clone https://github.com/LINUX-OASIS/NBD-MOUNT-VDI-QCOW.git
    ```
2.  Navigate to the project directory:
    ```sh
    cd NBD-MOUNT-VDI-QCOW
    ```
3.  Make the script executable:
    ```sh
    chmod +x custom-NBD-MOUNT-VDI-QCOW.sh
    ```

### 🪄 Usage

Simply run the script with `sudo` or as a user with `sudo` privileges. The script needs elevated permissions to manage kernel modules and devices.

```sh
sudo ./custom-NBD-MOUNT-VDI-QCOW.sh
```

The script will guide you through an interactive menu to mount or unmount your disk images.

## 🐧 Compatibility

This script is designed for Linux distributions that use the `apt` package manager. It has been tested and is known to be compatible with:

*   !Debian
*   !Ubuntu
*   !Linux Mint
*   Other Debian derivatives.

## 💬 Contributing

Pull requests, issues, and suggestions are warmly welcomed! For major changes, please open an issue first to discuss what you would like to change.

See CONTRIBUTING.md for guidelines.

## 🌐 Links

| Type          | Link                                                                                             |
|---------------|--------------------------------------------------------------------------------------------------|
| **Issues**    | https://github.com/LINUX-OASIS/NBD-MOUNT-VDI-QCOW/issues       |
| **Pull Requests** | https://github.com/LINUX-OASIS/NBD-MOUNT-VDI-QCOW/pulls         |
| **Releases**  | https://github.com/LINUX-OASIS/NBD-MOUNT-VDI-QCOW/releases     |
| **Wiki**      | https://github.com/LINUX-OASIS/NBD-MOUNT-VDI-QCOW/wiki           |

## 📜 License

This project is distributed under the **GNU General Public License v3.0**. See the `LICENSE` file for more information.

[!License: GPL v3](https://www.gnu.org/licenses/gpl-3.0)

## 🧙‍♂️ Maintainer

This project is maintained by:

**LINUX-OASIS**

---

*Happy Discomancing!* ✨
