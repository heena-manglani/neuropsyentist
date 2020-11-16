Customization


## **Oh My Zsh**
* Zsh is a terminal built on the same shell as bash and is now the default on Macs.
* Oh My Zsh is a framework that wraps around the zsh terminal and allows use of plugins and themes.

## Installation
To install Oh My ZSH:  
```bash
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

To install Powerlevel10k theme:  
```bash
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
```

To install plugins for the terminal:
* Auto suggestions
  ```bash
  git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
  ```
  * Auto highlighting commands
    ```bash
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
    ```
  * Auto completions
    ```bash
    git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions
    ```

## P10k fonts
The Powerlevel10k theme has recommended fonts to use although they are not necessary. <a href="https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k" target="_blank" rel="noreferrer">Install them here</a>


## Updating .zshrc

All of the configuration settings for OMZ will be in the ~/.zshrc file.
To update, in the terminal enter:
  ```bash
  nano ~/.zshrc
  ```
Add this into the plugins section:
    ```json
    plugins=(
            git
            zsh-autosuggestions
            zsh-syntax-highlighting
            zsh-completions
    )
    ```
To change the zsh_theme
```bash
ZSH_THEME="powerlevel10k/powerlevel10k"
```

* Anaconda