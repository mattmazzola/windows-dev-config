# Machine Configuration

## Testing

```powershell
winget configuration show -f .\configurations\settings.dsc.yaml
winget configuration show -f .\configurations\install.dsc.yaml
```

```powershell
winget configuration validate -f .\configurations\settings.dsc.yaml
winget configuration validate -f .\configurations\install.dsc.yaml
```

## Running

```powershell
winget configuration -f .\configurations\settings.dsc.yaml
winget configuration -f .\configurations\install.dsc.yaml
```

## Manual Setup

See [MANUAL.md](MANUAL.md)

## Links

- <https://learn.microsoft.com/en-us/windows/dev-home/setup>
- <https://learn.microsoft.com/en-us/windows/package-manager/configuration/>
