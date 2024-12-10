# Setup Guide for Nexus Node CLI
## On Windows
### 1. Install WSL (Windows Subsystem for Linux):
- Open **PowerShell** (Run as Administrator).
- Run the command
```
wsl --install
```
- Restart your computer after completion.
### 2. Install Ubuntu:
- Open Start Menu -> Launch Ubuntu.
- Set a password using:
```
passwd
```
_(Note: Password characters won't display as you type.)_
### 3. Install Rust:
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs/ | sh
```
### 4. Update APT & Install Dependencies:
```
sudo apt update && sudo apt upgrade
sudo apt install build-essential pkg-config libssl-dev git-all
```
### 5. Install Protocol Buffers:
```
sudo apt install -y protobuf-compiler
```
### 6. Install Nexus CLI:
```
curl https://cli.nexus.xyz/ | sh
```

## On Linux Ubuntu
### 1. Install Rust:
```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs/ | sh
```
### 2. Update APT & Install Required Dependencies:
```
sudo apt update && sudo apt upgrade
sudo apt install build-essential pkg-config libssl-dev git-all
sudo apt install -y protobuf-compiler
```
### 3. Install Nexus CLI:
```
curl https://cli.nexus.xyz/ | sh
```
