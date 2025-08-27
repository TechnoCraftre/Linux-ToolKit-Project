# Linux Toolkit Project 🐧

This project is a beginner-friendly **Linux mini-toolkit** to practice essential commands and workflows for every day usage.

---

## Project Goals
- Learn core Linux commands by building a small toolkit.
- Practice file management, user management, process monitoring, networking, and automation.
- Document everything in a GitHub repo.

---

## ⚙️ Toolkit Components
1. **Environment Setup**
   - Users: `dev1`, `test1`, `admin1` (`admin1` has sudo).
2. **File Management**
   - Directory: `/opt/linux_toolkit`
   - Subfolders: `logs/`, `bin/`
3. **System Monitoring**
   - `dummy_worker.py` (background script writing logs)
   - `process_report.txt` (saved running processes)
4. **Networking**
   - SSH server enabled
   - Commands: `ping`, `ss`, `ssh`
5. **Automation**
   - `rotate_logs.sh` script
   - `cronjob.txt` with daily rotation schedule

---

## Artifacts
- `process_report.txt`
- `cronjob.txt`
- Screenshots (commands in action)

---

## Essential Commands
This repo documents **25 must-know Linux commands** with **what, why, how** explanations.

| Command | What it does | Why it matters | How (example) |
|---------|--------------|----------------|---------------|
| `pwd`   | Show current directory | Navigate safely in scripts | `pwd` |
| `ls`    | List files/dirs | Quick check | `ls -lah /opt/linux_toolkit` |
| `cd`    | Change directory | Move into project folders | `cd logs` |
| `mkdir` | Create directory | Structure apps/logs | `mkdir logs` |
| `touch` | Create file | Seed logs/configs | `touch logs/app.log` |
| `cp`    | Copy file | Backup configs | `cp app.log app.bak` |
| `mv`    | Move/rename | Rotate logs | `mv app.bak app.1` |
| `rm`    | Remove file | Clean artifacts | `rm app.1` |
| `chmod` | Change permissions | Secure files | `chmod 640 app.log` |
| `chown` | Change owner | Ownership to user | `chown admin1:admin1 logs/` |
| `find`  | Search files | Locate configs/logs | `find . -name "*.log"` |
| `grep`  | Search text | Debug logs | `grep error app.log` |
| `tar`   | Archive/compress | Bundle backups | `tar -czf logs.tar.gz logs/` |
| `du`    | Disk usage | Check space hogs | `du -sh *` |
| `df`    | Disk free | Pre-deploy check | `df -h` |
| `ps`    | Show processes | Inspect running apps | `ps aux | head` |
| `top`   | Live process view | See CPU/memory usage | `top` |
| `kill`  | Stop process | End rogue app | `kill -9 <PID>` |
| `systemctl` | Service control | Start/stop services | `systemctl status ssh` |
| `journalctl` | View service logs | Debug daemons | `journalctl -u ssh` |
| `ping`  | Check connectivity | Test reachability | `ping google.com` |
| `ss`    | Socket stats | Check open ports | `ss -tulnp` |
| `ssh`   | Remote login | Connect to servers | `ssh admin1@host` |
| `crontab` | Schedule jobs | Automate tasks | `crontab -l` |

---

## How to Run
1. Clone this repo:
   ```bash
   git clone https://github.com/TechnoCraftre/Linux-ToolKit-Project.git
   cd linux-toolkit
