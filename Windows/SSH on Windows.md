## 1. Enable OpenSSH Server on Windows
- **Search** for "Apps & features" from the Start menu.
- **Select** "Optional Features" and then "Add a feature".
- **Find** and **install** "OpenSSH Server".

## 2. Check OpenSSH Server Service
- **Open** the "Services" app.
- **Ensure** the "OpenSSH SSH Server" is set to "Running". If not, **start** it manually.

## 3. Generate SSH Keys
- On the client machine, generate keys if you don't have them:
  ```
  ssh-keygen -t rsa -b 2048
  ```

## 4. Copy the Public Key to Windows
### Option 1: Using ssh-copy-id (Linux/Mac)
  ```
  ssh-copy-id -i ~/.ssh/id_rsa.pub username@windows-machine-ip
  ```
### Option 2: Manually
- **Copy** the public key data.
- On Windows, **navigate** to `C:\Users\YourUsername\.ssh` or create it if it doesn't exist.
- **Create** or edit the `authorized_keys` file and **paste** the public key data.

## 5. Set Correct Permissions
- **Right-click** on the `.ssh` folder and the `authorized_keys` file.
- **Set** permissions so that only your user account has full control.

## 6. Configure OpenSSH Server
- **Edit** the SSH server configuration file at `C:\ProgramData\ssh\sshd_config`:
  ```
  PubkeyAuthentication yes
  AuthorizedKeysFile .ssh/authorized_keys
  ```
- **Restart** the OpenSSH Server service if changes are made.

## 7. Test the Connection
- **Connect** from your client machine:
  ```
  ssh username@windows-machine-ip
  ```