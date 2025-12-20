# Contributing to Custom Themes

This is a personal repository, but here are some guidelines for adding new themes:

## Adding a New Theme

1. Create a new `.omp.json` file in the `themes/` directory
2. Name it descriptively (e.g., `my-custom-theme.omp.json`)
3. Ensure it follows the Oh My Posh schema
4. Test the theme before committing

## Theme Naming Convention

- Use lowercase with hyphens: `my-theme-name.omp.json`
- Include `.omp.json` extension for clarity
- Use descriptive names that reflect the theme's appearance or purpose

## Theme Requirements

- Must be valid JSON
- Should include the schema reference:
  ```json
  "$schema": "https://raw.githubusercontent.com/JanDeDobbeleer/oh-my-posh/main/themes/schema.json"
  ```
- Include `version: 2` for the latest Oh My Posh version

## Testing Your Theme

Before committing, test your theme:

```bash
# Validate JSON syntax
python3 -m json.tool themes/your-theme.omp.json

# Test the theme (if Oh My Posh is installed)
oh-my-posh init pwsh --config themes/your-theme.omp.json | Invoke-Expression
```

## Documentation

If you add a new theme, consider updating the `themes/README.md` file to include a brief description of your theme and its features.
