## **Oh My Zsh**
============

Zsh is a terminal built on the same shell as bash and it is now the default on all new Macs.
Oh My Zsh is a framework that wraps your zsh terminal and allows the use of plugins and themes to make your terminal.

## Installations
* Install Oh My ZSH:  
    ```bash
    sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    ```

* Install Powerlevel10k Theme:  
    ```bash
    git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
    ```

* Install Plugins:
  * Auto suggestions in the terminal
    ```bash
    git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
    ```

  * Auto Highlighting commands in the terminal
    ```bash
    git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
    ```

  * Auto Completions commands in the terminal
    ```bash
    git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions
    ```

## P10k fonts
The Powerlevel10k theme has recommended fonts to use although they are not necessary.  
Install them <a href="https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k" target="_blank" rel="noreferrer">here</a>


## Updating .zshrc

All of the configuration settings for OMZ will be in the ~/.zshrc file.
* In the terminal
    ```bash
    nano ~/.zshrc
    ```
* Add this into the plugins section
    ```json
    plugins=(
            git
            zsh-autosuggestions
            zsh-syntax-highlighting
            zsh-completions
    )
    ```
* Change the ZSH_THEME
    ```bash
    ZSH_THEME="powerlevel10k/powerlevel10k"
    ```

* Anaconda 