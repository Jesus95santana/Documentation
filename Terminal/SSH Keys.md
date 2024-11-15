  
## Prerequisites  
- SSH service must be running on the Host Machine.  
- You should have SSH access to the Host Machine.  
- Your SSH private and public key pair (`id_rsa` and `id_rsa.pub`) must be set up on your local machine.  
  
## Steps  
  
### 1. Ensure SSH is Running on Host Machine  
Make sure that the SSH service is running and enabled on your Host Machine. You can verify this by running the following command on the Host Machine:  
  
```bash  
sudo systemctl status sshd  
```  
  
The output should indicate that the `sshd` service is active and running.  
  
### 2. Copy SSH Key Using `ssh-copy-id`  
From your local machine (the one you want to SSH from), run the following command to copy your public key to the Host Machine:  
  
```bash  
ssh-copy-id -i ~/.ssh/id_rsa.pub username@hostmachine_ip  
```  
  
Replace `username` with your Host Machine’s username (typically `username`), and `hostmachine_ip` with the IP address of your Host Machine.  
  
Example:  
  
```bash  
ssh-copy-id -i ~/.ssh/id_rsa.pub username@192.168.0.12  
```  
  
When prompted, enter the password for the `username` user. After successful authentication, your SSH key will be added to the `~/.ssh/authorized_keys` file on the Host Machine.  
  
### 3. Manually Add the SSH Key (Alternative Method)  
If `ssh-copy-id` is not available or you prefer to manually add the key, follow these steps:  
  
#### a. Copy the Public Key from Local Machine  
On your local machine, display the contents of your SSH public key:  
  
```bash  
cat ~/.ssh/id_rsa.pub  
```  
  
Copy the entire output (starting with `ssh-rsa`).  
  
#### b. SSH into the Host Machine  
SSH into your Host Machine using the password method:  
  
```bash  
ssh username@192.168.0.12  
```  
  
#### c. Create `.ssh` Directory (if not already created)  
Once logged in, create the `.ssh` directory (if it doesn’t exist):  
  
```bash  
mkdir -p ~/.ssh  
chmod 700 ~/.ssh  
```  
  
#### d. Add the Public Key to `authorized_keys`  
Open the `authorized_keys` file (create it if it doesn’t exist) and paste the SSH public key you copied earlier:  
  
```bash  
nano ~/.ssh/authorized_keys  
```  
  
Paste the public key and save the file.  
  
Set the correct permissions for the `authorized_keys` file:  
  
```bash  
chmod 600 ~/.ssh/authorized_keys  
```  
  
### 4. Test SSH Access  
After completing the steps, try SSHing into your Host Machine again. This time, you should not be prompted for a password:  
  
```bash  
ssh username@192.168.0.12  
```  
  
If everything is set up correctly, you should be logged in without needing to enter a password.  
  
## Troubleshooting  
- Ensure that the `.ssh` directory and `authorized_keys` file have the correct permissions:  
- `.ssh` directory: `chmod 700 ~/.ssh`  
- `authorized_keys` file: `chmod 600 ~/.ssh/authorized_keys`  
- Double-check that the correct public key is in the `authorized_keys` file.  
- If you cannot access the Host Machine via SSH, verify that SSH is running (`sudo systemctl status sshd`). 