## Linux Command Line SOP

### Basic File Operations
- **List Directory Contents**
  ```
  ls
  ```
- **Change Directory**
  ```
  cd [directory]
  ```
- **Copy Files or Directories**
  ```
  cp [source] [destination]
  ```
- **Move or Rename Files or Directories**
  ```
  mv [source] [destination]
  ```
- **Remove Files or Directories**
  ```
  rm [file_or_directory]
  ```
- **Create a New Directory**
  ```
  mkdir [directory]
  ```

### File Viewing and Manipulation
- **View File Content**
  ```
  cat [file]
  ```
- **Display the first parts of files**
  ```
  head [file]
  ```
- **Display the last parts of files**
  ```
  tail [file]
  ```
- **Edit Files**
  ```
  nano [file]
  ```
- **Search Text Within Files**
  ```
  grep [pattern] [file]
  ```

### System Monitoring and Management
- **Display Disk Usage**
  ```
  df -h
  ```
- **Monitor System Processes**
  ```
  top
  ```
- **Display Who is Logged On**
  ```
  who
  ```
- **Kill a Process**
  ```
  kill [pid]
  ```

### Network Operations
- **Ping Host**
  ```
  ping [host]
  ```
- **Check Network Connections**
  ```
  netstat
  ```
- **Display Routing Table**
  ```
  route -n
  ```
- **Download Files**
  ```
  wget [url]
  ```
- **Transfer Files**
  ```
  scp [source] [user@host:destination]
  ```

### Package Management
- **Update Package Index**
  ```
  sudo apt update
  ```
- **Upgrade Installed Packages**
  ```
  sudo apt upgrade
  ```
- **Install a Package**
  ```
  sudo apt install [package]
  ```
- **Remove a Package**
  ```
  sudo apt remove [package]
  ```

### Permissions and Ownership
- **Change File Permissions**
  ```
  chmod [permissions] [file]
  ```
- **Change File Ownership**
  ```
  chown [owner]:[group] [file]
  ```

### Searching and Sorting
- **Find Files and Directories**
  ```
  find [directory] -name [search_pattern]
  ```
- **Sort File Contents**
  ```
  sort [file]
  ```

### Text Processing
- **Transform Text**
  ```
  tr [set1] [set2]
  ```
- **Compare Files**
  ```
  diff [file1] [file2]
  ```
- **Concatenate Files**
  ```
  cat [file1] [file2] > [newfile]
  ```

### System Information
- **Display Current Date and Time**
  ```
  date
  ```
- **Show System Information**
  ```
  uname -a
  ```
- **Print Working Directory**
  ```
  pwd
  ```

### Hardware Information
- **List USB Devices**
  ```
  lsusb
  ```
- **List PCI Devices**
  ```
  lspci
  ```

### Compression and Archives
- **Create a Tar Archive**
  ```
  tar -cvf [archive.tar] [files]
  ```
- **Extract a Tar Archive**
  ```
  tar -xvf [archive.tar]
  ```
- **Compress Files**
  ```
  gzip [file]
  ```
- **Decompress Files**
  ```
  gunzip [file.gz]
  ```

### Networking and Firewall
- **Enable Firewall**
  ```
  sudo ufw enable
  ```
- **Disable Firewall**
  ```
  sudo ufw disable
  ```
- **Add Firewall Rule**
  ```
  sudo ufw allow from [source] to [destination] port [port]
  ```
- **Display Firewall Status**
  ```
  sudo ufw status
  ```

### Disk and File System Management
- **List File Systems**
  ```
  lsblk
  ```
- **Check Filesystem Disk Space Usage**
  ```
  du -sh [directory]
  ```
- **Mount a File System**
  ```
  mount [device] [mount_point]
  ```
- **Unmount a File System**
  ```
  umount [mount_point]
  ```

### User and Group Management
- **Add a New User**
  ```
  sudo adduser [username]
  ```
- **Delete a User**
  ```
  sudo deluser [username]
  ```
- **Add a User to a Group**
  ```
  sudo adduser [username] [group]
  ```
- **Create a New Group**
  ```
  sudo addgroup [groupname]
  ```

### Miscellaneous
- **Create a Symbolic Link**
  ```
  ln -s [target] [link_name]
  ```
- **Display Calendar**
  ```
  cal
  ```