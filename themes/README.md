# Custom Oh My Posh Themes

This directory contains custom Oh My Posh theme configurations.

## Available Themes

### example-clean.omp.json
A clean and simple powerline-style theme featuring:
- Current directory path
- Git status with visual indicators
- Exit code status
- Time display on the right
- Simple prompt character

**Best for:** Minimal setup with essential information

### example-minimal.omp.json
A more feature-rich theme with:
- Username display
- Directory path with depth limit
- Detailed git information including stash count
- Node.js version display (when in a Node project)
- Python version display (when in a Python environment)
- Execution time for commands > 500ms
- Time display
- Enhanced visual style with diamonds and powerline

**Best for:** Development work with multiple language environments

## Using a Theme

To test a theme:

```bash
oh-my-posh init pwsh --config ./example-clean.omp.json | Invoke-Expression
```

Or for bash/zsh:

```bash
eval "$(oh-my-posh init bash --config ./example-clean.omp.json)"
```

## Customizing Themes

1. Copy an existing theme file
2. Modify the segments, colors, or symbols
3. Refer to the [Oh My Posh documentation](https://ohmyposh.dev/docs/configuration/overview) for all available options
4. Test your changes immediately

### Common Customizations

- **Colors:** Modify `foreground` and `background` properties
- **Symbols:** Change Unicode characters in `template` properties
- **Segments:** Add or remove blocks in the `segments` array
- **Layout:** Adjust `alignment` and `newline` properties

## Adding Your Own Themes

Simply create a new `.omp.json` file in this directory with your custom configuration.
