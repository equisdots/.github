<h1 align="center">
 equisdots 
</h1>

<p align="center">
  <em>An opinionated Arch-based desktop stack: Hyprland in the Lua era, a
  Quickshell shell, a live palette engine and a wallpaper kernel with
  interactive scenes.</em>
</p>

<p align="center">
  <a href="https://github.com/equisdots/dots">dots</a> ·
  <a href="https://github.com/equisdots/hyprland">hyprland</a> ·
  <a href="https://github.com/equisdots/shell">shell</a> ·
  <a href="https://github.com/equisdots/davincix">davincix</a> ·
  <a href="https://github.com/equisdots/palettes">palettes</a> ·
  <a href="https://github.com/equisdots/nyx">nyx</a> ·
  <a href="https://github.com/equisdots/background">background</a>
</p>

---

## What is equisdots

equisdots is the desktop behind **X Linux**: a set of small repositories that
install a complete, palette-driven environment on top of Arch Linux. One
command clones, wires and updates the whole stack; every piece follows the same
active palette, so the bar, window borders, widgets and wallpapers restyle
themselves live when the theme changes.

<!-- TODO(brand): add a desktop screenshot or GIF here (profile/assets/hero.png). -->

## Highlights

- **Hyprland, Lua era.** The compositor configuration is written against the
  Lua API (0.55+), with reusable modules for keybinds, rules, animations and
  colors.
- **Quickshell shell.** Bar with zones and a full editor, panels, popups and
  floating desktop widgets with a visual redactor; palette-aware everywhere.
- **Nyx.** The little mascot island / notch that turns into a control center:
  chibi species (flame, cat, dog, eyes, dots, watcher), typewriter clock, live
  stats, quick-action toggles and a searchable widget grid.
- **Live palette engine.** base16 palettes plus semantic roles; switching a
  palette recolors the shell, window borders, widgets and running scenes
  without a reload.
- **Wallpaper kernel with scenes.** `davincix` drives still images, video and
  interactive JavaScript scenes rendered by the `xwww` engine, with reveal
  transitions, a picker and lock-screen caching.
- **Small engines, one command.** `timex` (calendar and weather), `xturing`
  (terminal settings UI) and `login` (static SDDM theme) complete the stack.
  `dots` installs, updates and diagnoses everything.

## Install

```sh
bash <(curl -fsSL https://raw.githubusercontent.com/equisdots/dots/main/dots) setup
```

After the first run `dots` lives in `~/.local/bin`:

```sh
dots update   # pull every repo and re-deploy the payload
dots doctor   # check dependencies, clones and installed paths
```

## Repository map

| Repository | What it provides |
|---|---|
| [dots](https://github.com/equisdots/dots) | Meta installer and updater: clones, wires and updates the whole stack. |
| [hyprland](https://github.com/equisdots/hyprland) | Hyprland compositor configuration (Lua era), scripts and system installer. |
| [shell](https://github.com/equisdots/shell) | Quickshell shell: bar, editor, panels, popups and desktop widgets. |
| [nyx](https://github.com/equisdots/nyx) | Mascot island / notch + control center for the shell: species, dock, live stats and quick actions. |
| [davincix](https://github.com/equisdots/davincix) | Wallpaper kernel: images, video and interactive scenes, with the picker frontend. |
| [palettes](https://github.com/equisdots/palettes) | base16 color palettes with semantic roles and the schema they follow. |
| [theme-sync](https://github.com/equisdots/theme-sync) | Palette-driven theming engine for the applications in the stack. |
| [background](https://github.com/equisdots/background) | Wallpaper collection, published as a release asset, plus the interactive scene catalog. |
| [timex](https://github.com/equisdots/timex) | Time and weather engine: calendar popup, forecast and settings tab. |
| [xturing](https://github.com/equisdots/xturing) | Terminal UI (ratatui) for the settings panel: bar, zones, themes, monitors, input and widgets. |
| [login](https://github.com/equisdots/login) | Minimal static SDDM login theme. |

The `xwww` wallpaper daemon (a fork of awww with extra transitions) lives at
[x-ports/xwww](https://github.com/x-ports/xwww).

## Documentation

- [Interactive scene guide](https://github.com/equisdots/background/blob/main/docs/scene-guide.md):
  how to write, install and understand the JavaScript wallpapers.
- [Hyprland configuration](https://github.com/equisdots/hyprland/tree/main/docs)
  and [quick reference](https://github.com/equisdots/hyprland/blob/main/docs/quick-reference.md).
- [Shell windows and widgets](https://github.com/equisdots/shell/tree/main/docs)
  and [desktop widgets](https://github.com/equisdots/shell/blob/main/docs/desktop-widgets.md).
- [davincix](https://github.com/equisdots/davincix/tree/main/docs) and the
  [dots installer](https://github.com/equisdots/dots#readme).

## Contributing

Issues and pull requests are welcome in any repository. Each repo documents its
own workflow; see [CONTRIBUTING.md](https://github.com/equisdots/.github/blob/main/CONTRIBUTING.md)
and [SECURITY.md](https://github.com/equisdots/.github/blob/main/SECURITY.md)
for the org-wide rules.
