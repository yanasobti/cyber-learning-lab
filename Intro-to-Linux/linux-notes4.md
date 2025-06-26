# 🐧 Linux Day 4 - Summary

This README summarizes key Linux commands for package management and service control. It's perfect for revision or as a beginner-friendly cheat sheet!

---

## 📦 Package Management Tools

### 1. `dpkg` – Low-Level Debian Package Manager

  sudo dpkg -i <package.deb>                    # Install a .deb file
  sudo dpkg -r <package-name>                   # Remove a package

### 2.`apt` – Advanced Package Tool (Most Common)
  sudo apt update                               # Update package list
  
  sudo apt install <package-name>               # Install a package
  
  sudo apt remove <package-name>                # Remove a package
  
  sudo apt purge <package-name>                 # Remove package + config
  
  sudo apt upgrade                              # Upgrade installed packages
  
  sudo apt full-upgrade                         # Upgrade w/ dependencies

Useful apt commands:
  apt list --installed                          # List installed packages
  
  sudo apt edit-sources                         # Edit sources.list
  
  sudo apt -h                                   # Help menu
  
  sudo apt --list                               # List options


### 3.`aptitude` – Terminal-based GUI 

  sudo aptitude                                 # Launch aptitude interface


### 4.`snap` – App Store-like Package System

  sudo snap install --classic <pkg>             # Install snap app

  
### 🐍 Python & Ruby Package Managers
👉 Python (pip)
  pip3 install -v <package>

👉 Ruby (rubygems)
  gem install <package>

## 📘 Notes of the Day – Summary

Today's notes cover essential Linux package management tools and language-specific package installers. We explored dpkg, apt, aptitude, and snap for managing software on Debian-based systems. Commands for installing, removing, and updating packages were practiced. We also touched on Python's pip and Ruby's gem for handling dependencies in scripting environments. These tools are foundational for any Linux user or cybersecurity enthusiast working in real-world environments.
