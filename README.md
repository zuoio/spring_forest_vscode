# Spring Forest VSCode

Spring Forest and Night Forest are two Visual Studio Code color themes based on the palettes used by the Spring Forest JetBrains theme plugin.

## Themes

- **Spring Forest** — a light theme using the Islands Spring Forest palette.
- **Night Forest** — a dark theme using the Islands Night Forest palette.

The interface colors, editor colors, terminal ANSI colors, TextMate scopes, and semantic token colors are defined in:

```text
themes/Spring Forest-color-theme.json
themes/Night Forest-color-theme.json
```

## Run locally

1. Open this directory in Visual Studio Code.
2. Press `F5` to launch an Extension Development Host window.
3. Run **Preferences: Color Theme** and choose **Spring Forest** or **Night Forest**.
4. After editing a theme file, run **Developer: Reload Window** in the development host.

## Package the extension

Install `vsce` once, then run it from this directory:

```powershell
npm install --global @vscode/vsce
vsce package
```

This produces a `.vsix` file that can be installed from the Extensions view using **Install from VSIX...**.

The `publisher` value in `package.json` is currently `spring-forest`; replace it with your Marketplace publisher ID before publishing.
