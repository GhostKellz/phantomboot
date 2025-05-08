# 👻 phantomboot

[![Arch Linux](https://img.shields.io/badge/Arch-Linux-blue?logo=arch-linux&logoColor=white)](https://archlinux.org)
[![Btrfs](https://img.shields.io/badge/Filesystem-Btrfs-8BC34A?logo=linux&logoColor=white)](https://btrfs.readthedocs.io/)
[![Systemd Boot](https://img.shields.io/badge/Boot%20Manager-systemd--boot-292D3E?logo=systemd&logoColor=white)](https://www.freedesktop.org/wiki/Software/systemd/systemd-boot/)
[![Go](https://img.shields.io/badge/Written%20in-Go-00ADD8?logo=go&logoColor=white)](https://golang.org)
[![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🧠 Motivation

Everyone who's run Arch Linux long enough knows the **inevitable moment** — a failed boot, broken initramfs, corrupted NVIDIA DKMS install, or botched kernel upgrade. Whether it’s an update gone wrong or driver hell, getting your system back on its feet shouldn’t be a painful, cryptic mess.

**phantomboot** is a **bootable, modular CLI recovery environment** for Arch-based systems, with a heavy focus on **Btrfs**, **snapshots**, **Timeshift/Snapper integration**, and **DKMS troubleshooting**.

---

## ⚙️ Core Tech Stack

Go — main language for CLI logic + automation

Cobra — powerful CLI framework

Arch Linux — primary target OS

Btrfs — snapshot-aware FS with subvolume support

Systemd-boot — default bootloader focus (GRUB optional)

Snapper/Timeshift — snapshot creation and rollback

Zsh/Bash menus — interactive rescue CLI

--- 
## 🚀 Goal

Create a streamlined **rescue toolkit** that can be booted or chrooted into to:
- Restore Btrfs snapshots (Timeshift, Snapper)
- Rebuild initramfs or reinstall broken kernels
- Fix DKMS issues (especially NVIDIA Open/Proprietary)
- Mount btrfs subvolumes intelligently
- Handle broken `systemd-boot` configs
- Perform package rollbacks with pacman or custom scripts
- Backup/restore to/from remote (e.g., rsync to NAS or Minio)

---

## 🛠 Features (Planned)

- ✅ Modular command design using Cobra CLI
- 🔧 Snapshot auto-detection + restoration (Snapper + Timeshift)
- 🖥 DKMS module rebuild helper
- 🗃 Rsync-based manual backup/restore support
- 🖱 Basic TUI/CLI UI with BubbleTea (maybe down the road)
- 🔐 SSH-ready rescue mode (to fix remote boxes too!)
- 💾 Bootable ISO/USB creator (future milestone)

---

## 📦 Built With

- **Go** — main language for CLI and logic
- **Cobra** — CLI framework
- **Arch Linux** — target environment
- **Btrfs** — snapshot-aware filesystems
- **Systemd-boot** — default bootloader support

---

## 🤝 Contributing

Want to pitch in or suggest a recovery scenario we should support?

Feel free to:
- Submit PRs
- Open issues
- Share crash logs or failure cases

This tool is built **for Arch users, by Arch users** — we’ve all been there.

---

## 💀 Why "phantomboot"?

Because your rescue system should be like a ghost: **invisible until needed, then unstoppable** when summoned.

---

## 📜 License

MIT — because freedom matters.

