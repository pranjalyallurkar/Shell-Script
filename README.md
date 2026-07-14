# Shell-Script
 AWS EC2 Setup Automation

A Bash-based automation script that provisions a fresh Ubuntu EC2 instance by installing commonly used development tools and configuring essential services. This project simplifies the initial server setup for web applications and DevOps environments.

---

## Features

- Install and update system packages
- Install Git
- Install Docker Engine
- Install Nginx
- Install Node.js (LTS)
- Install Python 3 and Pip
- Configure UFW Firewall
- Enable HTTP (80), HTTPS (443), and SSH (22)
- Enable and start Docker
- Enable and start Nginx
- Display installed software versions
- Generate setup logs

---

## Tech Stack

- Bash Shell Scripting
- Ubuntu Linux
- AWS EC2
- Docker
- Nginx
- Git
- Node.js
- Python 3
- UFW Firewall

---

## Project Structure

```
aws-ec2-setup-automation/
│
├── setup.sh
├── logs/
│   └── setup.log
├── screenshots/
│   ├── docker-version.png
│   ├── nginx-running.png
│   └── firewall-status.png
└── README.md
```

---

## Prerequisites

- Ubuntu 22.04 or later
- AWS EC2 Instance
- Sudo privileges
- Internet connection

---

## Installation

Clone the repository



Move into the project directory

```bash
cd aws-ec2-setup-automation
```

Make the script executable

```bash
chmod +x setup.sh
```

Run the setup script

```bash
sudo ./setup.sh
```

---

## Installed Components

- Git
- Docker Engine
- Docker Compose Plugin
- Nginx
- Node.js LTS
- npm
- Python 3
- Python Pip
- UFW Firewall

---

## Firewall Configuration

The script automatically enables the following firewall rules:

| Service | Port |
|----------|------|
| SSH | 22 |
| HTTP | 80 |
| HTTPS | 443 |

---

## Services Started

- Docker
- Nginx

The script also enables these services to start automatically after system reboot.

---

## Verification

Check Docker version

```bash
docker --version
```

Check Git version

```bash
git --version
```

Check Node.js version

```bash
node -v
```

Check Python version

```bash
python3 --version
```

Check Nginx status

```bash
sudo systemctl status nginx
```

Check Docker status

```bash
sudo systemctl status docker
```

Check Firewall status

```bash
sudo ufw status
```

---

## Sample Output

```
Updating system...
Installing Git...
Installing Docker...
Installing Nginx...
Installing Node.js...
Installing Python...
Configuring Firewall...
Starting Services...

Setup Completed Successfully!

Git: v2.x.x
Docker: v28.x.x
Node.js: v22.x.x
Python: v3.x.x
Nginx: Active (running)
Firewall: Active
```

---

## Future Improvements

- Install MySQL
- Install PostgreSQL
- Install Java JDK
- Configure Swap Memory
- Install Certbot
- Deploy a React application automatically
- Deploy a Django application automatically
- Install Docker Compose
- Configure AWS CLI automatically
- Add rollback support on installation failure

---

## Learning Outcomes

- Linux Administration
- Bash Shell Scripting
- AWS EC2 Management
- Service Management using systemctl
- Firewall Configuration using UFW
- Docker Installation and Management
- Nginx Configuration
- Server Provisioning Automation

---

## Author

**Pranjal Yallurkar**

Computer Science Engineering Student

Skills: AWS | Linux | Bash | Docker | Kubernetes | React | Django | DevOps

---

## License

This project is licensed under the MIT License.
