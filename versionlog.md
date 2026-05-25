# Version Log

All project changes should be recorded here whenever the theme is updated.

## v0.0.8

- Updated the visible theme version in `metrics.ini` using `WindowTitle=INTIFADA v0.0.8`.
- Updated `README.md` before commit to reflect the current command-menu and modifier-detector work.
- Rebuilt the ScreenCommandMenu background as its own BGAnimation with header, frame, profile, modifier detector, silent music, and blank out transition handling.
- Tuned ScreenSelectMusic style-icon exit commands and the options message exit animation.
- Expanded the PIU modifier detector to include SuperShuffle in alternate states and Blind in judge states.
- Fixed the noteskin detector condition so `NXA-HIDDEN` still requires P1 to be human before drawing P1 frames/shines.
- Added Player 2 PIU modifier detector layers across frames, shines, speed, noteskins, display, path, alternate, judge, and rush modules, with right-side positions ordered Speed through Rush and human-player guards for each side.
- Added generic `setstate,13` combination badges for Display, Path, Alternate, and Judge whenever more than one mod in that category is active, with a BGM-synced pulse effect using `effectmagnitude,1,1.2,0` and `effectperiod,1`.

## v0.0.7

- Updated the visible theme version in `metrics.ini` using `WindowTitle=INTIFADA v0.0.7`.
- Updated `README.md` before commit to reflect the current ScreenSelectMusic style display and modifier detector work.
- Replaced the built-in ScreenSelectMusic current-mode text with BGAnimation-driven style icons for single, double, halfdouble, and versus states, including a halfdouble difficulty icon asset.
- Switched player status and PIU mod detector BGAnimation conditions from load-time `Condition`/`Cond` to per-frame `DrawCond` so enabled-player and modifier visuals can update while screens remain loaded.
- Imported the PIU modifier detector into the OperatorMenu background and refreshed the ScreenSelectMusic/MainMenu/OperatorMenu BGAnimation behavior.
- Removed the local ScreenSelectMusic cur-mode bitmap font in favor of a redirect, removed unused `_options page` assets, and allowed language strings to fall back through the theme stack.
- Tuned ScreenSelectMusic difficulty list sizing, hidden-difficulty handling, and global bitmap text shadow defaults.
- Replaced the shared menu music loop asset.
- Ignored local `BGAnimation - Copy.ini` editor backup files so they stay out of commits.

## v0.0.6

- Updated the visible theme version in `metrics.ini` using `WindowTitle=INTIFADA v0.0.6`.
- Updated `README.md` before commit to reflect the current version and latest ScreenOptions/OperatorMenu work.
- Reworked ScreenOptions layout metrics for centered long-row option values, explanation text placement, frame animation, line highlight behavior, hidden player names/icons, and more/exit-row commands.
- Redirected ScreenOptions item/title/explanation fonts through theme font redirs and replaced the bullet/underline/cursor/line-highlight assets used by the options interface.
- Rebuilt the OperatorMenu background as a BGAnimation folder with header, frame, footer, player, and info layers, and updated related back/page redirs.
- Expanded `Languages/english.ini` with option titles, option explanations, option names, and updated system credit labels for the options screens.
- Replaced ScreenOptions navigation/toggle/change sounds, restored difficulty easier/harder audio assets, and updated shared menu music assets.
- Removed local duplicated fallback sections and assets now inherited from `!CMPIU`, including ScreenCredit, ScreenDemonstration, ScreenOptionsMaster, CustomScoring, FadingBanner, FadingBackground, and SongManager definitions.
- Added pump touch-control graphics and `TouchControlPump` coordinate metrics.
- Removed completed ScreenOptions and ScreenPlayerOptions items from `roadmap.txt`.
- Expanded the local AI BGAnimation notes with guidance for using font/text layers in BGAnimation files.

## v0.0.5

- Updated the visible theme version in `metrics.ini` using `WindowTitle=INTIFADA v0.0.5`.
- Updated `README.md` before commit to reflect the current version and latest font/credit asset cleanup.
- Removed unused ScreenCredit background logo/sprite art from `BGAnimations/ScreenCredit background/`.
- Removed the unused `OptionIcon` font definition and texture.
- Removed the local `_piusystem` font definition and texture so remaining `_piusystem` redirs resolve through the `!CMPIU` fallback theme.

## v0.0.4

- Updated the visible theme version in `metrics.ini` using `WindowTitle=INTIFADA v0.0.4`.
- Updated `README.md` before commit to reflect the current version and latest cleanup/stability focus.
- Added `halfdouble` to the one-player mode list for ScreenSelectMusic.
- Restored ScreenSelectMusic `PrevScreen` to `ScreenProducer` instead of looping back into ScreenSelectMusic.
- Forced ScreenSelectMusic ModeMenu actions through `group,ALL MUSIC` before changing sort to avoid empty-wheel crashes.
- Reduced the ScreenSelectMusic SortMenu to `GROUP` and `TITLE`, and disabled section headers in the wheel.
- Cleared CodeDetector banner group inputs to prevent banner-group codes from firing.
- Tuned `EditDifficultyMeter` by setting two meter digits and hiding the description text.
- Removed unused or superseded ScreenSelectMusic graphics, old doubled-resolution difficulty icons, score frames, autogen/background-frame files, unused sound aliases, old menu timer art, and unused movie/audio assets.
- Moved the difficulty list cursor texture into `Graphics/_common/` and updated both player cursor sprites to reference the shared path.
- Simplified the failed gameplay BGAnimation after removing the old `STAGEBREAK` movie layer.

## v0.0.3

- Updated the visible theme version in `metrics.ini` using `WindowTitle=INTIFADA v0.0.3`.
- Updated `README.md` before commit to reflect the current version and ScreenSelectMusic overlay work.
- Added ScreenSelectMusic overlay section-change glow and direction-aware arrow layers driven by `MusicWheelDirection()`.
- Routed ScreenSelectMusic overlay `Moving`, `Section`, and `Settled` metrics through BGAnimation layer commands with `playcommand`.
- Disabled the old disc frame command-driven animation path after moving the behavior into the overlay BGAnimation.
- Added `Create a splash` to `roadmap.txt`.
- Removed ignored/local-only item references from `README.md` so the GitHub-facing overview only describes tracked project content.
- Added the public README rule to the local AI collaboration guide so ignored/local-only files stay out of GitHub-facing documentation.

## v0.0.2

- Updated the visible theme version in `metrics.ini` using `WindowTitle=INTIFADA v0.0.2`.
- Updated `README.md` before commit to reflect the current version and recent documentation focus.
- Preserved the local ignored AI collaboration guide and private folder reference convention.
- Included the current ScreenSelectMusic background frame asset path changes in the committed workspace state.

## v0.0.1

- Initialized the theme version in `metrics.ini` using `WindowTitle=INTIFADA v0.0.1`.
- Added `versionlog.md` as the canonical change log for future updates.
- Added `AI.md` to document project collaboration rules and theme development conventions.
- Consolidated the project-local StepMania AMX theme skill guidance into `AI.md`.
- Added `README.md` to describe the project for GitHub viewers.
- Added `.gitignore` and ignored `AI.md`.
- Established that each commit initializes a new version section in `versionlog.md`.
- Established that `README.md` must be updated before every commit.
- Added `accessible-folders.md` to track folder paths available for project reference checks.
- Added `G:\PROGRAMS\stepmania-amx` as a reference-only source path for StepMania AMX.
- Added `folders.md` to ignored files.
- Researched the StepMania AMX source and expanded the local AI theming guidance with metrics, asset resolution, actor command, BGAnimation, and screen flow notes.
- Updated `README.md` to clarify that local AI notes and private folder lists are ignored.
- Expanded the local AI actor command documentation with detailed syntax, command categories, examples, and editing guidance.
- Added brief examples to each documented actor command in the local AI guidance.
- Added expected behavior notes to each documented actor command in the local AI guidance.
- Added possible values for documented actor commands that use non-numeric string parameters.
- Added a Lua expression reference for actor command dispatch conditions based on registered StepMania AMX Lua functions.
- Documented the source-backed `DrawCond` BGAnimation layer key and how it differs from `Cond`/`Condition`.
- Added fixed-value references for non-boolean Lua expression returns such as play modes, coin modes, difficulty enums, grade enums, and music wheel direction.
- Expanded the BGAnimation guidance with source-backed explanations of top-level keys, layer conditions, imports, layer command dispatch, sprite/particle/tile behavior, repeat timing, camera/rendering keys, and practical usage patterns.
- Added a source-backed screen type reference describing the compiled screen classes and what each one is useful for during theme development.
- Added a source-backed CodeDetector reference covering code syntax, all configured code items, player modifier effects, screen-specific uses, scroll speed list behavior, and AMX source quirks.
- Expanded the CodeDetector notes with a detailed explanation of `SortMenu` and `ModeMenu`, including music wheel metrics, action syntax, valid sort orders, examples, and caveats.
- Expanded the `ModeMenuActions` guidance with all parsed ModeChoice commands, accepted values, examples, validity checks, and how `sort,<SortOrder>` interacts with MusicWheel.
