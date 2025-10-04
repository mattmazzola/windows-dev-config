# Computer Setup

## Enable Features

- Windows Hypervisor Platform
- Hyper-V
- Windows Subsytem for Linux

> Restart to complete

- Install wsl
- Install wsl Distribution
    ```pwsh
    wsl --install Ubuntu-22.04
    ```

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
```

## More Configuration

- Configure Terminal Settings
    - Set start directory to Dev Drive
    - Change default to cross platform powershell (NOT Windows Powershell)
- Setup oh-my-posh
    - `oh-my-posh font install meslo`
    - [Update terminal settings to use font](https://ohmyposh.dev/docs/installation/fonts#configuration)
    - Update VSCode use settings to use font: `"terminal.integrated.fontFamily": "MesloLGM Nerd Font"`
    - [Update $PROFILE to se oh-my-posh prompt](https://ohmyposh.dev/docs/installation/prompt)








Processor	Intel(R) Xeon(R) W-3245 CPU @ 3.20GHz, 3192 Mhz, 16 Core(s), 32 Logical Processor(s)
Installed Physical Memory (RAM)	256 GB
Adapter Description	NVIDIA Quadro RTX 4000
