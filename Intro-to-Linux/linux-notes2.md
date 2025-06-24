# 🔐 Linux – Day 2 Summary

📅 Date: June 23, 2025   
📁 This session focused on user creation, sudo privileges, system information,
file operations, and using Linux’s built-in help tools — all practiced in Kali Linux 🐧.


### File_operations:
  - command: "📄 cp file1 file2"
    description: "Copies file1 to file2."
  - command: "🗑️ rm filename"
    description: "Removes or deletes a file."
  - command: "🔍 which bash"
    description: "Shows the location/path of a shell or command."
  - command: "📊 ps"
    description: "Displays current running processes and your active shell."

### System_info:
  - command: "🧑‍💻 id"
    description: "Displays UID, GID, and group membership of the current user."
    example: "uid=1000(yana) gid=1000(yana) groups=1000(yana),27(sudo)"

  - command: "💻 hostname"
    description: "Displays the computer’s hostname (name in a network)."
    example: "kali"

  - command: "🧠 uname"
    description: "Prints system/kernel information."
    variations:
      - flag: ""
        meaning: "Prints kernel name (usually 'Linux')"
      - flag: "-a"
        meaning: "All system info: kernel, version, machine"
      - flag: "-n"
        meaning: "Network node hostname"
      - flag: "-m"
        meaning: "Machine hardware (e.g., x86_64)"
      - flag: "-p"
        meaning: "Processor type (may be 'unknown')"
    example: "Linux kali 6.3.0-kali1-amd64 #1 SMP x86_64 GNU/Linux"

  - command: "🔎 apropos user"
    description: "Searches man pages for commands related to a keyword."
    example: |
      adduser (8) – add a user to the system
      useradd (8) – create a new user

  - command: "📘 man chmod"
    description: "Displays the manual/help page for any command."
    tip: "Press 'q' to exit the manual."

### Sudo_privileges:
  description: >
    👑 `sudo` stands for "superuser do" and allows regular users to run commands as root.
    It's essential for system administration, user management, and installing software.
    
  commands:
  
    - "👤 sudo adduser <username>"
      description: "Adds a new user with guided setup."
      
    - "🔐 sudo passwd <username>"
      description: "Sets or changes a user’s password."
      
    - "❌ sudo deluser <username>"
      description: "Deletes a user account."
      
    - "🔄 sudo su - <username>"
      description: "Switches to another user's shell session."
      
    - "🛡️ sudo visudo"
      description: "Safely edit the sudoers file with syntax checking."

### Visudo_info:
  purpose: "🧾 Grant sudo access safely using visudo"
  
  example_line: "yana ALL=(ALL:ALL) ALL"
  
  meaning:
  
    - "yana: Username being granted sudo access"
    
    - "ALL=(ALL:ALL): Can act as any user/group"
    
    - "ALL: Can run all system commands"
    
  warning: "⚠️ Never edit /etc/sudoers directly! Use 'sudo visudo' only."


## NOTES
  - "✅ Practiced adding, deleting, and switching users"
  - "📖 Explored the use of man pages and apropos for help"
  - "🔍 Used uname, id, hostname to explore system info"
  - "💬 Confirmed shell environment using which and ps"


## Screenshots of the terminal of some commands used


![20250625_001035](https://github.com/user-attachments/assets/9c1c36d3-4e47-4991-ad87-b23d30c89382)
~using cp and rm command
![20250625_001345](https://github.com/user-attachments/assets/b2ae0a7d-05e4-4c94-bef1-2f68f85e5bf6)
~using uname -all, ps and hostname
![20250625_001611](https://github.com/user-attachments/assets/af273352-ae67-4185-ac0a-73f50c8a190e)

![20250625_001628](https://github.com/user-attachments/assets/cb0704b4-061e-4661-b480-8fb14618f259)

![20250625_001820](https://github.com/user-attachments/assets/18a2a1c3-8719-4834-89e3-1784367f319b)
~showing the visudo text editor
