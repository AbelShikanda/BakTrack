# BakTrack

**BakTrack** is an offline versioning system designed to help you track, organize, and back up files to a portable storage device efficiently. It allows you to efficiently manage file versions without requiring an internet connection.

## Features

✅ **Offline Versioning** – Keep track of file changes without an internet connection.  
🔍 **Difference Checking** – Compare local files with backup storage before syncing.  
🛠 **Automated Backups** – Push updates to your backup drive with a simple command.  
🔐 **User-Based Access** – Configure different backup users for better security.  
🚀 **Portable & Efficient** – Designed for external USB drives and other storage devices.

## 📥 Installation

You can install **BakTrack** using **npm** (recommended) or manually from GitHub.

### 🟢 Install via npm (Recommended)

Ensure you have **Node.js** (>=14) and **npm** installed. Then run:

npm i baktrack
sudo npm i -g baktrack

This installs **BakTrack** globally, allowing you to use it from anywhere.

### 🟠 Install from GitHub (Manual)

Alternatively, you can clone the repository and set it up manually:

git clone https://github.com/AbelShikanda/baktrack.git

cd baktrack

chmod +x bin/\*

To make `bak` available system-wide:

For **bsh** users:

echo 'export PATH="$HOME/baktrack/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc

For **zsh** users:

echo 'export PATH="$HOME/baktrack/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc

## 🚀 Usage

### 🔹 Initialize a Backup in the directory you want to backup

bak init

Creates the necessary `.bak` configuration folder.

### 🔹 Set a Backup User

bak config <username>

### 🔹 Insert your backup device

bak config set device <name>
bak config set mount </mount/point>

### 🔹 Create the backup

bak config create backup

### 🔹 Push Changes to Backup

bak track

### 🔹 Check for Differences Before Syncing

bak check

### 🔹 Restore from Backup

bak restore

## 🔄 Updating BakTrack

To update **BakTrack** when installed via npm:

npm update -g baktrack

If installed from GitHub:

cd baktrack
git pull origin main

## 🛠 Contributing

Feel free to open an issue or submit a pull request if you’d like to contribute to **BakTrack**.

## 📜 License

MIT License © 2025 Abel Shikanda
