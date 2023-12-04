# Watermelon

1. Install Dependencies
   1. Termux
        ```shell
        { pkg up
        pkg install git tmux zsh ;}
        ```
   1. Alpine
        ```shell
        apk add --upgrade --no-cache git tmux zsh
        ```
   1. Ubuntu
        ```shell
        { apt update
        apt install git tmux zsh ;}
        ```

1. Installing
    ```shell
    { git clone --depth 1 https://github.com/cchristion/watermelon.git
    cd watermelon
    cp -rsv $(pwd)/.config ~/
    cp -rsv $(pwd)/.zshenv ~/.zshenv
    mkdir -p ${XDG_CACHE_HOME:-$HOME/.cache}/zsh ${XDG_CONFIG_HOME:-$HOME/.config}/zsh/plugins
    cd ;}
    ```

1.  Installing fast-syntax-highlight plugin for zsh
    ```shell
    git clone --depth 1 https://github.com/zdharma-continuum/fast-syntax-highlighting ${XDG_CONFIG_HOME:-$HOME/.config}/zsh/plugins/fast-syntax-highlighting
    ```

1.  Installing powerlevel10k theme
    ```shell
    git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${XDG_CONFIG_HOME:-$HOME/.config}/zsh/plugins/powerlevel10k
    ```
