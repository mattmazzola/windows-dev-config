# Computer Setup

## Enable Features

- Windows Hypervisor Platform
- Hyper-V
- Windows Subsytem for Linux

> Restart to complete

### WSL

- Install wsl
  - Ensure version 2 is set (Should be latest by default)
- Install wsl Distribution

    ```pwsh
    wsl --install Ubuntu-22.04
    ```

### Other

- Open application "Phone Link" to initialize installation

## Configuration

- Enable Dark mode theme
- Enable Developer Mode
  - Enable Settings
    - Show file extensions
    - Show hidden files
    - Show empty drives
    - Show End Task
    - Show full path in title
    - Show task view button
    - Show hidden files
    - Never hide task bar labels
- Enable Dev Home
- Create Dev Drive (100 GB+)
- Enable Clipboard History
  - Enable history sync across devices

## Installation

```pwsh
winget install Microsoft.PowerShell
winget install Git.Git
winget install Microsoft.VisualStudioCode
winget install JanDeDobbeleer.OhMyPosh
winget install Docker.DockerDesktop
winget install GitHub.cli
winget install OBSProject.OBSStudio
winget install NickeManarin.ScreenToGif
winget install Microsoft.PowerToys
winget install Logseq.Logseq
```

## More Configuration

These steps require installation of some applications above

- Configure Terminal Settings
  - Set start directory to Dev Drive
  - Change default to cross platform powershell (NOT Windows Powershell)
- Setup oh-my-posh
  - `oh-my-posh font install meslo`
  - [Update terminal settings to use font](https://ohmyposh.dev/docs/installation/fonts#configuration)
  - Update VSCode use settings to use font: `"terminal.integrated.fontFamily": "MesloLGM Nerd Font"`
  - [Update $PROFILE to se oh-my-posh prompt](https://ohmyposh.dev/docs/installation/prompt)

## Setup Git Aliases

### Ensure Git editor is set to code

```pwsh
git config core.editor "code --wait"
```

### Copy Git Config

Copy [gist](https://gist.githubusercontent.com/mattmazzola/7a6350df0a0d27a62137d14572340229/raw/d2431e1f672546fb6267e8307c699fb80ef03bc5/.gitconfig) of git config and manually merge with your existing config using `git config --edit`

For the bash version (in WSL), ensure xclip is installed: `sudo apt install xclip`

```pwsh
$GIT_CONFIG_URL = "https://gist.githubusercontent.com/mattmazzola/7a6350df0a0d27a62137d14572340229/raw/d2431e1f672546fb6267e8307c699fb80ef03bc5/.gitconfig"
Invoke-WebRequest -Uri $GIT_CONFIG_URL | Select-Object -ExpandProperty Content | Set-Clipboard
```

```bash
sudo apt -y update && sudo apt install -y xclip
```

```pwsh
git config --edit
```

```bash
GIT_CONFIG_URL="https://gist.githubusercontent.com/mattmazzola/7a6350df0a0d27a62137d14572340229/raw/d2431e1f672546fb6267e8307c699fb80ef03bc5/.gitconfig"
curl -o /tmp/.gitconfig $GIT_CONFIG_URL
cat /tmp/.gitconfig | xclip -selection clipboard
rm /tmp/.gitconfig
```

## Optional (SSH setup)

```pwsh
ssh-keygen -t ed25519

# Copy public key to clipboard
cat ~/.ssh/id_ed25519.pub | Set-Clipboard

# Add key to service such as Github, GitLab, etc.
```

## Setup LogSeq

### Create LogSeq Directory for Graph

```pwsh
md D:\LogSeq
```
