# GTA V Cherax Lua Projects

A curated archive of my GTA V Cherax Lua projects, experiments, release builds, tools, and development notes.

Created by **Public_Urinal / Animus**  
Discord: **animusx1337**  
GitHub: **https://github.com/ARandomAddonDev/GTAV-Cherax**

Estimated Development Time: **350+ hours** as of **06/26/2026**

---

## Overview

This repository collects Lua-based projects created for **GTA V Cherax**.

The goal is to preserve development progress, organize release builds, document major systems, and keep a clean public-facing reference for my Cherax work.

Projects in this repository may include:

- Drift and vehicle handling systems
- DriftGod development and release builds
- Drift tuning and preset experiments
- Stunt and trick systems
- Garage / saved vehicle tools
- HUD and quick menu experiments
- Ghost replay and race systems
- PTFX / particle effect testing
- SuperDrive and momentum experiments
- Road surface / grip experiments
- Utility scripts
- Minigame-style concepts
- Notes, changelogs, and archived tests

Some scripts are polished.  
Some scripts are experimental.  
Some scripts are kept for reference or future rebuilds.

Use each build with that in mind.

---

## Featured Project: DriftGod

**DriftGod** is a Cherax Lua drifting project focused on making GTA V drifting feel more stylish, arcade-like, expressive, and customizable.

The project is inspired by older mod-menu drifting systems from the Impulse / 2Take1 era, but expanded into its own progression-focused drift system with presets, tuning, HUDs, stunts, ghost races, unlocks, and experimental utilities.

DriftGod is not intended to be a perfect simulation drift system.

It is meant to feel:

- Fun
- Fast to use
- Stylish
- Tunable
- Progression-driven
- Showcase-friendly
- Easy to iterate on
- Built around real in-game testing

---

## DriftGod Preview

YouTube preview:

```txt
https://www.youtube.com/watch?v=0s6jtqomePs&t=9s
```

---

## DriftGod Core Features

Depending on the build, DriftGod may include:

- Custom drift tuning
- Built-in drift presets
- Custom preset save/load support
- Automatic last-preset restore on load
- Custom preset priority over automatic built-in preset switching
- Score-based preset unlocks
- DriftGod Garage saved vehicle HUD
- Stunt HUD / Stunt Menu
- Score-based stunt cooldowns
- Stunt unlock and progression systems
- Ghosts & Race beta tools
- Saved ghost recording and playback
- Race countdown and race result tools
- HUD position controls
- Saved HUD hotkeys
- PTFX / particle effect experiments
- SuperDrive beta tools
- Road Surface / Grip beta tools
- Challenge and reward pages
- Build/version logging
- Intro and loading UI experiments
- Single-file release builds

Features may change between builds because DriftGod is still actively being developed.

---

## Current DriftGod Focus

Recent DriftGod development has focused on:

- Cleaner Home, Garage, Settings, and Arcade UI organization
- Drift presets restoring automatically on load
- Custom presets staying prioritized over built-in unlocks
- Garage HUD and Stunt HUD saved hotkeys
- Default hotkeys:
  - **Garage HUD:** Insert
  - **Stunt HUD:** Home
- Ghosts & Race subtab cleanup
- Score-based stunt cooldowns
- Reduced debug/noise in release-style builds
- Keeping risky experimental features labeled as beta

---

## Default HUD Hotkeys

DriftGod may assign saved hotkeys for frequently used HUDs.

```txt
Garage HUD default: Insert
Stunt HUD default: Home
```

These can be changed from DriftGod settings when the build supports saved hotkey dropdowns.

Typical HUD controls:

```txt
Garage HUD:
  Arrow keys  = select
  Enter/Right = spawn/open
  Delete      = back out or close
  F5          = scan saved vehicles

Stunt HUD:
  Arrow keys = select
  Enter      = run selected stunt
  Delete     = back out or close
```

---

## Ghosts & Race

**Ghosts & Race** is a beta system for recording, replaying, and racing against drift routes.

Depending on the build, it may include:

- Ghost recording
- Saved recording scan/load
- Playback controls
- Race setup
- Race countdown
- Checkpoints
- Finish / Did Not Finish controls
- Basic result tracking
- Ghost and replay settings

This system is still experimental and may change quickly.

---

## Garage

**DriftGod Garage** is the saved vehicle / quick spawn system.

Depending on the build, it may include:

- Saved vehicle scanning
- Random saved vehicle spawning
- Garage HUD quick menu
- Saved HUD position
- Saved HUD hotkey
- Vehicle preview placeholder / future preview support

The Garage system is intended to make vehicle access faster without cluttering the main menu.

---

## Stunts

DriftGod includes a stunt and trick system designed for arcade-style vehicle movement.

Depending on the build, stunts may include:

- Stunt menu / quick HUD
- Unlockable stunt categories
- Score-based cooldown progression
- Landing handling
- Safety caps
- Rotation tricks
- Flip tricks
- Donuts
- Advanced stunt experiments
- Per-build tuning changes

The goal is to make stunts feel fun without letting them spam or stack on top of themselves.

---

## Experimental / Beta Features

Some DriftGod systems are intentionally labeled as beta because they may be unstable.

Examples may include:

- SuperDrive
- Camera-based movement experiments
- WASD movement experiments
- Vehicle-based SuperDrive
- Road Surface / Grip experiments
- PTFX effects
- Ghosts & Race

Beta features may crash, behave inconsistently, or change between builds.

Use them carefully.

---

## Release Types

Projects in this repository may use release tags to make development status clear.

### ALPHA

**ALPHA** builds are active development builds.

They may include:

- New systems
- Debug tools
- Partially tested features
- Prototype code
- Known rough edges
- Fast-changing behavior

### BETA

**BETA** builds are more stable than alpha builds, but may still contain bugs.

They are intended for wider testing once major systems mostly work.

Example:

```txt
DriftGod v6.13.xx BETA
```

### RELEASE

**RELEASE** builds are intended to be cleaner public builds.

They should have:

- Less debug spam
- Cleaner menus
- More consistent behavior
- Better documentation
- Fewer experimental leftovers

Example:

```txt
DriftGod v1.0.0 RELEASE
```

---

## Built Releases vs Development Files

Some projects may include both release files and development files.

### Built Releases

Built releases are usually one large Lua file designed for easy loading.

Example:

```txt
releases/
  DriftGod.lua
```

A built release may be generated from multiple smaller files.

The goal of a built release is convenience:

- Easier to load
- Easier to upload
- Easier to share
- Better for platforms that expect one Lua file

### Development Files

Development files may be organized into folders such as:

```txt
DriftGod/
  core/
  systems/
  ui/
  data/
  assets/
```

This makes larger projects easier to maintain, debug, and rebuild.

---

## Assets

Some scripts may use external assets such as images, icons, logos, or other media.

Example:

```txt
Documents/Cherax/Lua/DriftGod/assets/
```

DriftGod may use assets for:

- Loading screens
- Logo display
- HUD visuals
- Notification experiments
- Ghost/race visuals
- Other UI tests

Assets may be:

- Included in the repository
- Stored in an assets folder
- Downloaded/cached by the script
- Disabled in certain single-file builds

If a build requires assets, that build should explain where they belong.

---

## Suggested Repository Structure

The repository may evolve, but a clean structure could look like:

```txt
GTAV-Cherax/
  README.md

  releases/
    DriftGod.lua

  DriftGod/
    core/
    systems/
    ui/
    data/
    assets/

  tools/
    builder/

  docs/
    changelogs/
    notes/
```

Possible folder purposes:

```txt
core/       Base config, state, save, utility, boot logic
systems/    Gameplay systems such as drift, stunts, SuperDrive, grip
ui/         Menus, HUDs, overlays, loading UI
data/       Presets, trick lists, ranks, tips, unlocks
assets/     Images, icons, logos, media files
releases/   Built one-file Lua releases
tools/      Builder scripts or helper tools
docs/       Notes, changelogs, development logs
```

---

## Building Single-File Lua Releases

Some projects may eventually use a builder script that combines modular files into one Lua release.

Example:

```txt
Input:
DriftGod/core/config.lua
DriftGod/systems/drift.lua
DriftGod/systems/stunts.lua
DriftGod/ui/menu.lua

Output:
releases/DriftGod.lua
```

A builder may:

- Read files in the correct load order
- Combine modules into one Lua file
- Preserve version/build information
- Keep required startup logic
- Exclude private or debug-only files
- Create cleaner release builds

This allows development to stay organized while still supporting single-file Lua releases.

---

## AI Assistance Transparency

Some parts of these projects were developed with assistance from AI tools such as ChatGPT.

AI was used as a coding assistant for:

- Prototyping
- Refactoring
- Debugging
- Documentation
- Build organization
- Code cleanup
- Error investigation
- Testing ideas faster

The project concepts, feature direction, in-game testing, tuning choices, cleanup decisions, and final behavior were manually directed and reviewed.

These scripts are not intended to be blind AI-generated dumps.

They are shaped through:

- Manual testing
- Cherax logs
- In-game behavior checks
- Repeated bug fixing
- Feature removal when something does not work
- Iterative tuning
- Community feedback
- Practical Cherax testing

AI is used as a tool, not as a replacement for testing or ownership.

---

## Development Notes

This repository may contain projects at different stages.

Some files may be:

- Experimental
- Deprecated
- Partially tested
- Kept for reference
- In active development
- Intended only for debugging
- Older versions preserved for comparison

Development builds may include debug logs, test menus, or systems that are later removed.

Release builds should be cleaner and may remove:

- Debug spam
- Broken experiments
- Duplicate systems
- Test-only buttons
- Old fallback code
- Prototype behavior

---

## Code Style Goals

The long-term goal is to keep larger projects readable, searchable, and consistent.

Preferred style:

```lua
DG.SuperDriveTick()
DG.ApplyExperimentalGrip()
DG.StartIntroHud()
DG.ClampStuntForce()
DG.ResetRunState()
```

The `DG.` namespace keeps DriftGod functions grouped and easier to find.

Good comments should explain **why** something exists, especially when it came from a bug, crash, or design change.

Example:

```lua
-- Past issue:
-- A/D yaw assist made steering feel unnatural, so DriftGod no longer
-- modifies A/D. GTA handles normal steering now.
```

The goal is not to over-comment obvious code.

The goal is to document important decisions, fixes, and lessons learned.

---

## Startup Logs and Build Info

DriftGod builds may print version information when loaded.

Example:

```txt
============================================================
DRIFTGOD
Drift Like a God
============================================================
Author: Animus / Public_Urinal
Discord: animusx1337
Version: v6.13.xx
Channel: ALPHA
Build: 2026.xx.xx.xxx
Last Updated: 2026-xx-xx
============================================================
```

Useful log fields include:

- Script name
- Author
- Discord username
- Version
- Build channel
- Build number
- Last update date

This helps identify which build someone is using when reporting issues.

---

## Credits

Created by:

```txt
Public_Urinal / Animus
Discord: animusx1337
```

Special thanks to:

- The GTA V modding community
- The Cherax Lua community
- People who provide testing ideas, feedback, and native references
- Community members who help explain Lua and Cherax behavior
- Anyone who reports bugs, shares logs, or helps improve the project

---

## Disclaimer

These scripts are provided for educational, archival, and personal modding purposes.

Use at your own risk.

I am not responsible for:

- Game crashes
- Broken sessions
- Lost settings
- Corrupted configs
- Unexpected behavior
- Bans
- Account issues
- Network issues
- Conflicts with other Lua scripts
- Conflicts with Cherax updates
- Conflicts with GTA V updates

Scripts may break after updates to GTA V, Cherax, Lua APIs, natives, or related tools.

Always test carefully.

---

## Reporting Issues

When reporting issues, include:

```txt
Script name
Version
Build channel
Build number
Cherax log
What you were doing
What happened
Whether other Lua scripts were loaded
Screenshots or clips if useful
```

Good reports make bugs much easier to reproduce and fix.

---

## Final Notes

This repository is a work in progress.

Some projects are polished.  
Some projects are experimental.  
Some projects are archived for reference.

The main goal is to document, preserve, and improve my GTA V Cherax Lua work over time.

Use the correct build type:

```txt
ALPHA   = experimental / active development
BETA    = testing / mostly working
RELEASE = stable public build
```

And always check the build notes before testing a new version.
