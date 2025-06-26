# 🐧 Linux Day 5 - Summary

📅 Date: June 26, 2025

🧠 Linux Services & Process Management

---
## 🔍 View Running Processes

  ps aux | grep <program>     # Find running process
  
  htop                        # Interactive process viewer
  
## 🔧 Controlling systemd Services

sudo systemctl stop <service>       # Stop a service

sudo systemctl start <service>      # Start a service

sudo systemctl restart <service>    # Restart a service

sudo systemctl reload <service>     # Reload config without restart

sudo systemctl disable <service>    # Disable on boot

sudo systemctl enable <service>     # Enable on boot

sudo systemctl status <service>     # Check service status

###💡 Example:

sudo systemctl stop sshd

sudo systemctl restart apache2

sudo systemctl enable nginx

## ❌ Kill a Running Service or Process
sudo kill <PID>                 # Kill a process by PID

sudo killall <process-name>     # Kill all instances by name

You can find the PID using:

  ps aux | grep <program>
  
## 🔄 Restart System or Shutdown
sudo reboot                    # Reboot the system

sudo poweroff                  # Power off the system

## 📂 Check Service Enable/Disable Status
systemctl is-enabled <service>

## ⏱ Check System Boot Time

uptime

systemctl status               # Shows last boot at bottom

## 🔎 Analyze Boot Performance
systemd-analyze

systemd-analyze blame          # Show services sorted by boot time

## 📘 What I Learned
Today, I learned how to monitor, manage, and control system services and processes in Linux using powerful tools like ps, htop, and systemctl. I explored how to start, stop, restart, enable, disable, and check the status of services managed by systemd. I also practiced identifying running processes and killing them using commands like kill and killall. These skills are essential for maintaining system stability, troubleshooting issues, and managing resources effectively on any Linux-based system.
