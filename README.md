# Custom Debian ISO with Preinstalled Applications

This repository contains scripts and configuration files to build a custom Debian ISO with GitHub Desktop, Visual Studio Code, Google Chrome, and Zoom preinstalled.

## Build Process

### Prerequisites

- Debian system for building the ISO.
- Required packages: `git`, `live-build`, `cdebootstrap`, `squashfs-tools`, `xorriso`.

### Steps to Build

1. **Setup Environment**
   ```bash
   sudo apt update
   sudo apt install git live-build cdebootstrap squashfs-tools xorriso

2. **Follow the steps**
Follow the steps from this github repository

3.**Preinstall Applications**
Download GitHub Desktop, VSCode, Google Chrome, and Zoom .deb packages.
Place them in config/includes.chroot/.
Add package names to config/package-lists/my.list.chroot.

4.**Customize and Build ISO**
Build the ISO:
sudo lb build

## Usage
### Boot and Install from ISO
Create a bootable USB drive or mount the ISO in a virtual machine.
Follow the installation prompts to install the custom Debian system.

### Verify Installed Applications
After installation, verify the functionality of preinstalled applications:

Open GitHub Desktop, VSCode, Google Chrome, and Zoom to ensure they work correctly.
