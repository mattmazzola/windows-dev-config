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

## Optional (SSH setup)

## Setup LogSeq

