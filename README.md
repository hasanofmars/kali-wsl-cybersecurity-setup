# Kali Linux WSL Cybersecurity Setup

A complete cybersecurity learning environment for Windows using Kali Linux on WSL.

## Install Kali Linux on WSL

```bash
wsl --install -d Kali-Linux
```

After installation, launch Kali and update the system:

```bash
sudo apt update && sudo apt full-upgrade -y
```

## Install Essential Security Tools

```bash
sudo apt install -y \
nmap \
wireshark \
tcpdump \
netcat-traditional \
curl \
wget \
git \
python3-pip \
john \
hydra \
sqlmap \
nikto \
gobuster \
dirb \
whois \
dnsutils \
net-tools \
masscan
```

## Install Development Tools

```bash
sudo apt install -y \
build-essential \
golang \
rustc \
cargo \
nodejs \
npm
```

## Install Python Security Libraries

```bash
pip3 install --user \
requests \
scapy \
pwntools \
impacket
```

## Verify Installation

```bash
nmap --version
sqlmap --version
john --list=formats
python3 -c "import scapy; print('Scapy installed successfully')"
```

## Optional: Install Kali Default Package

```bash
sudo apt install -y kali-linux-default
```

## Notes

* WSL is excellent for learning cybersecurity, scripting, and CTFs.
* Some wireless tools require real hardware or a virtual machine.
* Always practice only on systems you own or have permission to test.

## Recommended Learning Platforms

* Hack The Box
* TryHackMe
* OWASP
