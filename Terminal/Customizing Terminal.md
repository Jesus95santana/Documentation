## 1. Install Zsh
Zsh is a prerequisite for Oh My Zsh, so it must be installed first.

```bash
sudo apt update
sudo apt install zsh
```

## 2. Make Zsh the Default Shell
Change your default shell to Zsh.

```bash
chsh -s $(which zsh)
```

Log out and log back in for the change to take effect.

## 3. Install Oh My Zsh
Install the Oh My Zsh framework using curl or wget.

```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Or using wget:

```bash
sh -c "$(wget https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh -O -)"
```

## 4. Install the Powerlevel10k Theme
Clone the Powerlevel10k theme into the Oh My Zsh themes directory.

```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

## 5. Configure the Theme
Edit the `.zshrc` file to set Powerlevel10k as your theme.

```bash
nano ~/.zshrc
```

Change the line:

```plaintext
ZSH_THEME="powerlevel10k/powerlevel10k"
```

Save and exit (`CTRL+X`, then `Y`, then `Enter`).

## 6. Apply Changes
Source the `.zshrc` file or log out and log back in to apply changes.

```bash
source ~/.zshrc
```

## 7. Configure Powerlevel10k
When you start a new terminal session, the Powerlevel10k configuration wizard will start automatically. Follow the prompts to customize your prompt.
