# CMPIU

CMPIU is the shared StepMania AMX fallback theme for this theme set. Other custom themes can inherit from the `!CMPIU` folder through their `FallbackTheme` setting, using it as a common base for assets, metrics, sounds, fonts, and language strings.

This repository stores the fallback theme files for the `!CMPIU` theme folder.

## Project Structure

- `metrics.ini` - Main StepMania theme configuration, screen flow, and behavior map.
- `BGAnimations/` - Shared screen animation assets and redirects.
- `Fonts/` - Shared theme font assets.
- `Graphics/` - Shared theme images and interface graphics.
- `Languages/` - Shared localization files.
- `Sounds/` - Shared theme audio assets.
- `versionlog.md` - Change history for fallback theme updates.

## Current Baseline

- Theme folder: `!CMPIU`
- Role: fallback/base theme for other custom themes
- Repository branch: `main`
- Current documented version: `v0.0.3`
- Local window-title version marker: not currently defined in `metrics.ini`

## Shared Behavior

- Extra Stage 1 and Extra Stage 2 "try extra" evaluation sounds redirect to the shared `_silent` sound.
- Command menu speed options default to `P500` and provide AV-style speed choices from `P400` through `P700`, followed by classic X-speed choices.
- The display menu uses `static` for `BGAOFF`, and Rush options no longer force random background or save-score modifiers.
- The command menu includes a `PortraitTheme` configuration row.
- English and Spanish command-menu strings are provided for the shared option rows and AV speed names.

## Change Tracking

Record meaningful fallback theme changes in `versionlog.md`. Changes made here can affect any theme that inherits from `!CMPIU`, so document shared behavior, asset, language, and metric updates clearly.
