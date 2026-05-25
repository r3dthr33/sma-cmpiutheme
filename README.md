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
- Initial version log entry: `v0.0.1`
- Local window-title version marker: not currently defined in `metrics.ini`

## Change Tracking

Record meaningful fallback theme changes in `versionlog.md`. Changes made here can affect any theme that inherits from `!CMPIU`, so document shared behavior, asset, language, and metric updates clearly.
