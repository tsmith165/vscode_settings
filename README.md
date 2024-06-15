# VSCode Configuration

This repository contains the configuration files for setting up Visual Studio Code with your preferred settings and extensions.

## Prerequisites

-   Visual Studio Code installed on your system.
-   Git installed on your system.

## Setup Instructions

1. Clone this repository to your local machine:

```
git clone https://github.com/tsmith165/vscode_settings.git ~/.vscode_settings
```

2. Copy the `settings.json` file to your VSCode user settings directory:

-   **Windows (PowerShell)**: `Copy-Item -Path "~/.vscode_settings/settings.json" -Destination "$env:APPDATA\Code\User\settings.json"`
-   **MacOS (Terminal)**: `cp ~/.vscode_settings/settings.json "$HOME/Library/Application Support/Code/User/settings.json"`
-   **Linux (Terminal)**: `cp ~/.vscode_settings/settings.json "$HOME/.config/Code/User/settings.json"`

3. Open a terminal or command prompt and navigate to the cloned repository directory.

4. Run the following command to install the extensions listed in the `extensions.txt` file:

-   **Windows (PowerShell)**: `Get-Content ~/.vscode_settings/extensions.txt | ForEach-Object { code --install-extension $_ }`
-   **macOS/Linux (Bash)**: `cat ~/.vscode_settings/extensions.txt | xargs -L 1 code --install-extension`

5. Restart Visual Studio Code for the changes to take effect.

Your Visual Studio Code should now be set up with your preferred settings and extensions.
