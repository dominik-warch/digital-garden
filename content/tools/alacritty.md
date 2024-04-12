---
title: Alacritty
---
[Alacritty](https://alacritty.org/) ist ein schneller und leicht konfigurierbarer Terminal Emulator. Ich schwanke immer mal wieder zwischen Alacritty und [Kitty](https://sw.kovidgoyal.net/kitty/), bleibe aber öfter an Alacritty hängen.

## Konfiguration
Basierend auf zwei Dateien (einmal Theme, einmal alles anderen) unter `~/.config/alacritty/`

```toml
# alacritty.toml
import = ["~/.config/alacritty/rose-pine.toml"]

[window]
padding = { x = 10, y = 10 }
opacity = 0.95

## Only in Tiling WM
# decorations = "None"


[font]
size = 12.0

[font.bold]
family = "Hack Nerd Font Mono"
style = "Bold"

[font.bold_italic]
family = "Hack Nerd Font Mono"
style = "Bold Italic"

[font.italic]
family = "Hack Nerd Font Mono"
style = "Italic"

[font.normal]
family = "Hack Nerd Font Mono"
style = "Regular"

[keyboard]
bindings = [
  { key = "Return", mods = "Control|Shift", action = "SpawnNewInstance" }
]
```

```toml
# rose-pine.toml
# Colors section of "Alacritty - TOML configuration file format"
# https://github.com/alacritty/alacritty/blob/master/extra/man/alacritty.5.scd#color

[colors.primary]
foreground = "#e0def4"
background = "#191724"
dim_foreground = "#908caa"
bright_foreground = "#e0def4"

[colors.cursor]
text = "#e0def4"
cursor = "#524f67"

[colors.vi_mode_cursor]
text = "#e0def4"
cursor = "#524f67"

[colors.search.matches]
foreground = "#908caa"
background = "#26233a"

[colors.search.focused_match]
foreground = "#191724"
background = "#ebbcba"

[colors.hints.start]
foreground = "#908caa"
background = "#1f1d2e"

[colors.hints.end]
foreground = "#6e6a86"
background = "#1f1d2e"

[colors.line_indicator]
foreground = "None"
background = "None"

[colors.footer_bar]
foreground = "#e0def4"
background = "#1f1d2e"

[colors.selection]
text = "#e0def4"
background = "#403d52"

[colors.normal]
black = "#26233a"
red = "#eb6f92"
green = "#31748f"
yellow = "#f6c177"
blue = "#9ccfd8"
magenta = "#c4a7e7"
cyan = "#ebbcba"
white = "#e0def4"

[colors.bright]
black = "#6e6a86"
red = "#eb6f92"
green = "#31748f"
yellow = "#f6c177"
blue = "#9ccfd8"
magenta = "#c4a7e7"
cyan = "#ebbcba"
white = "#e0def4"

[colors.dim]
black = "#6e6a86"
red = "#eb6f92"
green = "#31748f"
yellow = "#f6c177"
blue = "#9ccfd8"
magenta = "#c4a7e7"
cyan = "#ebbcba"
white = "#e0def4"
```

