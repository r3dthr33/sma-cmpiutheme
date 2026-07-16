# CMPIU Version Log

All meaningful CMPIU fallback theme changes should be recorded here when the theme is updated.

## v0.0.4

- Removed `no static` from `RushDefault`, leaving the default Rush state as `1.0xmusic` only.
- Updated `README.md` to clarify that individual Rush rate choices apply `static` while the default Rush state does not force that display modifier.

## v0.0.3

- Changed the command-menu speed row to default to `P500` and added AV-style `P400` through `P700` choices before the classic X-speed options.
- Changed `BGAOFF` to use the `static` modifier instead of `randombg`.
- Removed forced `randombg` and `savescore` modifiers from Rush choices so they only change music rate.
- Added `PortraitTheme` as a command-menu configuration row.
- Added Spanish command-menu language strings and trimmed English strings to the shared command-menu entries used by CMPIU.
- Added `ScreenAttract` back navigation to `ScreenProducer`.
- Updated `README.md` to describe the new shared option behavior and language baseline.

## v0.0.2

- Added `ScreenEvaluation try extra1.redir` and `ScreenEvaluation try extra2.redir`.
- Redirected both Extra Stage evaluation prompts to `_silent`, suppressing those sounds for themes that inherit from CMPIU.
- Updated `README.md` to describe the shared evaluation-sound behavior.

## v0.0.1

- Initialized `versionlog.md` for the CMPIU fallback theme.
- Initialized `README.md` with CMPIU project identity, folder structure, baseline state, and change-tracking notes.
- Clarified in `README.md` that CMPIU is the shared fallback/base theme for other custom themes.
- Recorded the current repository baseline as the initial CMPIU import.
- Preserved the existing StepMania theme structure with `BGAnimations`, `Fonts`, `Graphics`, `Languages`, `Sounds`, and `metrics.ini`.
- Noted that `metrics.ini` currently does not define a local `WindowTitle` version marker.
