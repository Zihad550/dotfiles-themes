# dotfiles-themes

Colour themes for [Zihad550/dotfiles](https://github.com/Zihad550/dotfiles).
Each top-level folder is one theme. `colors.toml` is the palette; everything
the templates render (terminal, Hyprland, Quickshell and similar configs) is
generated on the machine and ignored here.

The dotfiles setup keeps a partial, sparse clone at `~/.dotfiles-themes`:
the theme picker lists every folder in this repo, and picking one checks out
only that folder.

```bash
df-theme-fetch --sync        # clone or refresh the index
df-theme-available           # list themes in this repo
df-theme-fetch rose-pine     # check out one theme
df-theme-set rose-pine       # apply it
```

## Adding a theme

Create `<name>/colors.toml` with `accent`, `cursor`, `foreground`,
`background`, `selection_foreground`, `selection_background` and
`color0`–`color15`, or with Omarchy's semantic names (`red`, `bright_blue`,
`muted`, `selection`, `mode = "light"`, ...). Optional files: `light.mode`, `icons.theme`,
`neovim.lua`, `vscode.json`, `obsidian-border-theme.json`.
