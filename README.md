# CMINTIFADA

CMINTIFADA is a custom StepMania AMX theme in early development. It is built around the standard StepMania theme folder layout and currently falls back to `!CMPIU`.

## Current Version

The visible theme version is stored in `metrics.ini` through the window title:

```ini
WindowTitle=INTIFADA v0.0.8
```

## Project Structure

- `metrics.ini` - Main StepMania theme configuration, screen flow, and behavior map.
- `BGAnimations/` - Screen animation assets and scripts.
- `Fonts/` - Theme font assets.
- `Graphics/` - Theme images and interface graphics.
- `Languages/` - Localization files.
- `Movies/` - Video assets.
- `Numbers/` - Number font assets.
- `Other/` - Miscellaneous theme files.
- `Sounds/` - Theme audio assets.
- `roadmap.txt` - Pending development tasks.
- `versionlog.md` - Change history for project updates.

## Theme Defaults

- Fallback theme: `!CMPIU`
- Target resolution: `1280x720`
- Current version: `v0.0.8`

## Development Status

This theme is currently a work in progress. Recent work has focused on ScreenSelectMusic stability, mode/sort menu behavior, custom ScreenOptions/OperatorMenu presentation, command-menu presentation, dynamic style indicators, and a PIU-style modifier detector with expanded noteskin, alternate, display, and judge coverage. Planned work includes editor support, score save/display screens, transitions, intro logo animation, improved two-player command display, and a splash screen.

## Change Tracking

All meaningful project changes should be recorded in `versionlog.md`. Version changes should also update the `WindowTitle` value in `metrics.ini`.

Before each commit, update this README so the GitHub-facing project description stays current with the committed state.
