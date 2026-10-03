# Contributing to equisdots

Thanks for taking the time to improve the stack. These rules apply to every
repository in the organisation; each one may add its own notes in a local
`CONTRIBUTING.md`.

## Where to report

Open the issue in the repository that owns the behaviour:

- installation, updates, packages, login theme: [dots](https://github.com/equisdots/dots)
- compositor configuration, keybinds, scripts: [hyprland](https://github.com/equisdots/hyprland)
- bar, panels, widgets, editor: [shell](https://github.com/equisdots/shell)
- wallpapers, scenes, picker: [davincix](https://github.com/equisdots/davincix) and
  [background](https://github.com/equisdots/background)
- colors and theming: [palettes](https://github.com/equisdots/palettes) and
  [theme-sync](https://github.com/equisdots/theme-sync)

If you are not sure, use the org-wide template and pick the component there.

## Pull requests

1. Keep the change focused: one topic per pull request.
2. Commit messages follow the existing style (`feat:`, `fix:`, `docs:`,
   `chore:`, `ci:`) with a short imperative subject.
3. Run the checks of the repository you touch (`cargo test`, `qmllint`,
   `bash -n`, whatever the repo documents) before opening the pull request.
4. Update the repository `CHANGELOG.md` when it exists; releases are cut by the
   maintainers from those entries.
5. New files default to the licenses already used by the repository (code is
   MIT-style unless stated otherwise; wallpapers and documentation follow the
   background repository terms).

## Style

- Documentation is written in English.
- Configurations and scripts should stay palette-driven: read the active
  palette instead of hardcoding colors.
- Prefer the small, existing helpers of each repository over new dependencies.
