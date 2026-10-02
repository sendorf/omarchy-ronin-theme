# ronin for Omarchy

A dark [Omarchy](https://omarchy.org/) theme built from one wallpaper: cold
teal water, and a single hot ember orange-red for the lantern and the ronin's
glasses. Deep teal surfaces, warm sand text, and restrained ember accents
create a cold, quiet workspace.

![ronin theme preview](preview.png)

## Highlights

- Native Omarchy dark mode through `mode = "dark"`
- Deep teal terminal and editor surfaces with warm sand text
- Matching generated colors for terminals, editors, browsers, Hyprland, and the
  Omarchy shell
- Ember focus states and cool syntax colors
- Cold teal ronin wallpaper
- Matching Yaru red icons

## Install

Install directly from the public Git repository:

```bash
omarchy theme install https://github.com/sendorf/omarchy-ronin-theme
```

Or paste the repository URL into **Install > Style > Theme** from the Omarchy
menu, then select it.

You can also copy this directory into `~/.config/omarchy/themes/ronin` and run:

```bash
omarchy theme set ronin
```

## Terminal transparency

Omarchy intentionally discards terminal configuration files from remotely
installed themes and safely regenerates them from `colors.toml`, so downloaded
copies use your normal terminal-opacity setting.

## Palette

The palette is not invented. Most accents were sampled from the wallpaper,
which is almost entirely two colour families — teal (`#16737A`, `#2A6B7E`,
`#3FB0B8`…) and ember (`#C4321F`, `#D4562D`, `#E8562F`…). The theme follows
that split: teal carries every background and structural surface, ember carries
everything that draws the eye.

| Role | Color |
| --- | --- |
| Background | `#051116` |
| Foreground | `#E3D3BE` |
| Accent | `#D4562D` |
| Selection | `#5C2317` |
| Muted | `#4D6B72` |
| Bright cyan | `#3FB0B8` |

Backgrounds run `#010608` → `#0A2C35`. Foregrounds are warm sand, so the teal
reads as cold by comparison.

`dark_foreground`, `muted` and the un-prefixed `red`/`blue`/`magenta`/`cyan` sit
around 3:1 against `background`. That is intentional: they are the dim half of
each ANSI pair, and every one of them has a `bright_` counterpart above 5:1.

## What's in it

- `colors.toml` — the palette, in Omarchy's semantic format
- `backgrounds/1-ronin.png` — the wallpaper, unmodified. `omarchy theme bg next`
  cycles it.
- `icons.theme` — `Yaru-red`
- `preview.png` — the wallpaper, shown in the theme switcher
- `LICENSE`

Every app config (Alacritty, Foot, Kitty, Ghostty, Neovim, Helix, VS Code,
Chromium, btop, Obsidian, tmux, and the rest) is generated from `colors.toml` by
Omarchy at theme-apply time, so none of those files are shipped here.

## Wallpaper

The wallpaper is AI-generated and carries no third-party rights. It is
distributed under this repository's MIT License along with the rest of the
theme.

## Disclaimer

This is an unofficial fan-made desktop theme, not affiliated with or endorsed
by Omarchy or Basecamp.

See [LICENSE](LICENSE) for licensing details.
