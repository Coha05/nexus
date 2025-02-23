# Setup Guide for Nexus Node CLI on TESTNET II
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
sudo apt install build-essential pkg-config libssl-dev git-all unzip
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
sudo apt install -y protobuf-compiler & unzip
```
```
wget https://github.com/protocolbuffers/protobuf/releases/download/v24.4/protoc-24.4-linux-x86_64.zip
unzip protoc-24.4-linux-x86_64.zip -d ~/protoc
sudo mv ~/protoc/bin/protoc /usr/local/bin/
sudo mv ~/protoc/include/* /usr/local/include/
```
### 3. Create screen
```
screen -S nexus
```
### 4. Install Nexus CLI:
```
curl https://cli.nexus.xyz/ | sh
```
### 5. Useful commands
- Exit screen: Ctrl A + D
- Access screen:
```
screen -r nexus
```
