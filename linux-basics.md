## 1.Terminal Commands

### Terminal is the way of communication without GUI.

### ls (List): List the files in the folder. (ls -la shows hidden files) 
### cd (Change Directory): Manage transitions between the folders. (cd .. moves to the parent folder).
### mkdir (Make Directory): Creates a new folder.
### grep (Global Regular Expression Print): Searches for text within a file. It is especially used for debugging in log files.
### chmod (Change Mode): Changes file permissions (Read,Write,Execute)
### top (Table of Processes): Shows system performance and which programs are using how much RAM/CPU.

## 2.Package Management (apt,pacman,dnf)

### In Linux,programs are installed from the internet via "Package Managers" instead of .exe files. The manager depends on the Linux distribution (Ubuntu,Arch,Fedora).

### apt (Debian/Ubuntu): The most common one. For example: sudo apt install python3.
### pacman (Arch Linux): Lighter and faster.
### dnf (Fedora/RedHat): A modern and smart package manager.

### Note: These tools automatically solve the other libraries (dependencies) that the program needs to be installed.

## 3.File Permissions

### Linux is a multi-users system; therefore, security is built on "Permissions". Every file has three types of permissions: Read(r) ,Write(w), and Execute (x).

### This permissions are defined for User,Group and Others separately.

### For instance, the chmod +x script.py command makes the file executable.

## 4.Services (systemctl)

### Programs (databases,web services, etc.) that always run in the background are called services. systemctl is the main command that manages these services.
### systemctl start/stop: Starts or stops the service.
### systemctl status: Shows whether the service is running or not at the moment.

## Why is Linux commonly preferred?

### It is open-source,meaning users can change and optimize everything, including the operating system kernel. 
### Permissions are very strict in Linux.So, it is really low to get a blue screen or system crash. 
### Everything can be installed from the terminal with one line in seconds.
### More than %90 of the servers in the world use the Linux. Therefore, users will be working in an environment that matches the industry standard.

