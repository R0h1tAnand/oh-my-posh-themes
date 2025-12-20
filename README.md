# Oh My Posh - Custom Themes

A personal repository to store and manage custom [Oh My Posh](https://ohmyposh.dev/) themes.

## About Oh My Posh

Oh My Posh is a custom prompt theme engine for any shell that can adjust the prompt string with a function or variable. It uses configuration files (JSON format) to define how your prompt should look.

## Repository Structure

```
oh-my-posh-themes/
├── themes/          # Custom theme files (.omp.json)
└── README.md        # This file
```

## Installation

### Prerequisites

1. Install Oh My Posh following the [official installation guide](https://ohmyposh.dev/docs/installation/windows)
2. Clone this repository:

```bash
git clone https://github.com/R0h1tAnand/oh-my-posh-themes.git
```

## Usage

### Using a Theme

To use any theme from this repository:

1. Navigate to the themes directory:
```bash
cd oh-my-posh-themes/themes
```

2. Apply a theme by pointing Oh My Posh to the theme file:

**PowerShell:**
```powershell
oh-my-posh init pwsh --config "path/to/oh-my-posh-themes/themes/your-theme.omp.json" | Invoke-Expression
```

**Bash/Zsh:**
```bash
eval "$(oh-my-posh init bash --config ~/path/to/oh-my-posh-themes/themes/your-theme.omp.json)"
```

### Making it Permanent

To automatically load your theme on shell startup:

**PowerShell:**
Add to your PowerShell profile (`$PROFILE`):
```powershell
oh-my-posh init pwsh --config "path/to/oh-my-posh-themes/themes/your-theme.omp.json" | Invoke-Expression
```

**Bash:**
Add to `~/.bashrc`:
```bash
eval "$(oh-my-posh init bash --config ~/path/to/oh-my-posh-themes/themes/your-theme.omp.json)"
```

**Zsh:**
Add to `~/.zshrc`:
```bash
eval "$(oh-my-posh init zsh --config ~/path/to/oh-my-posh-themes/themes/your-theme.omp.json)"
```

## Creating Custom Themes

1. Create a new `.omp.json` file in the `themes/` directory
2. Use the [Oh My Posh configuration documentation](https://ohmyposh.dev/docs/configuration/overview) to customize your theme
3. Test your theme using the commands shown above
4. You can use existing themes as templates or reference

### Useful Commands

- **Export current config:** `oh-my-posh config export --output themes/my-theme.omp.json`
- **Validate theme:** `oh-my-posh config validate --config themes/my-theme.omp.json`
- **Preview theme:** `oh-my-posh print primary --config themes/my-theme.omp.json`

## Resources

- [Oh My Posh Documentation](https://ohmyposh.dev/docs/)
- [Official Themes Gallery](https://ohmyposh.dev/docs/themes)
- [Configuration Guide](https://ohmyposh.dev/docs/configuration/overview)
- [Segment Documentation](https://ohmyposh.dev/docs/segments/overview)

## License

This is a personal repository. Feel free to use any themes as inspiration for your own customizations.