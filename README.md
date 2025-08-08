# Setup-and-Use-a-Firewall

## Objective
Configure and test firewall rules (block port 23, allow SSH).

## Environment
- OS:Kali Linux
- Tools: UFW (Linux), Windows Defender Firewall (PowerShell)

## Commands I ran

# Linux (UFW)
sudo ufw status verbose
sudo ufw allow ssh
sudo ufw enable
sudo ufw status numbered
sudo ufw deny 23/tcp
sudo ufw status numbered
sudo ufw delete deny 23/tcp

## Screenshots
- screenshots/-ufw-status.png
- screenshots/ubuntu-test.png

## Key findings
- Confirmed firewall rules block inbound TCP 23.
- Important: always allow SSH before enabling firewall remotely.
