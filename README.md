# Mellow for Bat
## Install Instructions
1. Create the configuration directory if it doesn't exist already
    ```sh
    mkdir -p "$(bat --config-dir)/themes"
    ```
2. Copy the theme file into the theme directory
    ```sh
    wget -P "$(bat --config-dir)/themes" "https://github.com/mellow-theme/bat/raw/refs/heads/master/mellow.tmTheme"
    ```
3. Rebuild bat's cache
    ```sh
    bat cache --build
    ```
4. Set mellow as your default theme
    ```sh
    echo '--theme="mellow"' >> $(bat --config-dir)/config
    ```
