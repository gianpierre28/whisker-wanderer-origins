![preview](https://raw.githubusercontent.com/gianpierre28/whisker-wanderer-origins/main/view_6dcbc49.svg)

# Nebula Prowler: Origins of the Stray Cosmos

Welcome to **Nebula Prowler**, a celestial sandbox adventure where you embody a lone feline astronaut who has lost all memory of its home planet. Your only companion is a malfunctioning AI collar that translates star charts into scent trails. As you leap between floating asteroids and derelict space stations, every gravity well you conquer reveals another fragment of your forgotten past. This is not just a platformer—it is an interactive meditation on memory, instinct, and the strange comfort of cosmic loneliness.

Unlike conventional cat games that focus on knocking things off shelves, Nebula Prowler flips the script. Here, your whiskers act as radar detectors, your purrs stabilize unstable quantum platforms, and your tail flicks can redirect meteor showers. The difficulty curve is not a wall—it is a gentle slope that begins with gentle moon hops and culminates in zero-gravity parkour across collapsing nebulae. Each level is hand-crafted to teach you a new environmental mechanic without a single tutorial text box, because real cats learn by doing.

The development philosophy behind this project is simple: a platformer should feel like a dance, not a chore. Every jump arc, every ledge grab, every pounce is calibrated through a proprietary physics engine that respects the weight of a digital feline body. The keyboard and gamepad inputs have been mapped with sub-frame precision, ensuring that a failed jump always feels like your mistake, never the game’s. As you progress, the world transforms from pastel-hued asteroid fields to crimson-tinged supernova remnants, each biome introducing a unique gravity modifier that keeps your reflexes honest.

This repository contains the complete source code for **Nebula Prowler**, including level design documents, shader source, audio cue files, and a custom dialogue system that lets the AI collar speak in riddles. Whether you are a curious player, a fellow game developer, or a cat lover with a passion for procedural generation, you will find something to sink your claws into here.

## Overview

![Unity Version](https://img.shields.io/badge/Unity-2026_LTS-gold) ![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-silver) ![Language](https://img.shields.io/badge/C%23-12.0-blue) ![License](https://img.shields.io/badge/License-MIT-green) ![Build Status](https://img.shields.io/badge/Build-Passing-brightgreen)

**Nebula Prowler** launched as a passion project in early 2025 and has evolved into a fully-fledged exploration game focused on the theme of self-discovery through environmental storytelling. The core loop deconstructs the classic platformer formula into a series of 'scent memory' puzzles: you collect glowing pollen spore clusters that, when combined, unlock neural maps of your cat’s prior life. The narrative is delivered through fragmented cutscenes that play in reverse chronological order, encouraging multiple playthroughs to piece together the true timeline.

The game supports three distinct control schemes: the classic keyboard layout, an Xbox controller preset, and a custom touch interface for players using handheld devices. Accessibility has been a priority from day one—every level includes an audio cue for incoming hazards, and a colorblind mode shifts all visual indicators to shape-based signals. The user interface is fully localized into Japanese, Spanish, and German, with community translations for French and Portuguese pending the next update.

**🎮 Gameplay Highlights:**
- **Gravity Ripple Mechanics:** Each level features a localized gravity field that you can temporarily invert by pressing and holding the grab button. This allows for ceiling-walking sections and mid-air redirects that feel remarkably natural.
- **Whisker Radar System:** A subtle visual pulse emanates from your cat’s whiskers every three seconds, briefly highlighting hidden paths, breakable walls, and secret collectible locations within a seven-meter radius.
- **Purr-Stabilizers:** When standing still on a trembling platform, your cat’s purr generates a resonance field that calms the shaking for four seconds—long enough to make a calculated leap.
- **Meteor Tail Redirect:** By double-tapping the jump button, your cat performs a tail spin that deflects incoming space debris into nearby energy crystals, triggering massive chain reactions.
- **Memory Echoes:** Scattered throughout the galaxy are ghostly afterimages of your past self. Touch them to witness short, non-interactive cutscenes that reveal who you were before the amnesia.

## Table of Contents

- [Getting Started](#getting-started)
- [Feature Matrix](#feature-matrix)
- [Globalization & Accessibility](#globalization--accessibility)
- [Physics & Feel](#physics--feel)
- [Architecture Overview](#architecture-overview)
- [Modding Support](#modding-support)
- [User Feedback & Iteration](#user-feedback--iteration)
- [Roadmap 2026](#roadmap-2026)
- [Contributing Guidelines](#contributing-guidelines)
- [Documentation & Resources](#documentation--resources)
- [Acknowledgments](#acknowledgments)
- [Sponsorship & Commercial Use](#sponsorship--commercial-use)
- [Disclaimer](#disclaimer)
- [License](#license)

## Getting Started

To bring Nebula Prowler to life on your own machine, you will need a 64-bit operating system (Windows 10/11, macOS Big Sur or newer, or any modern Linux distribution with Vulkan support), at least 8 GB of RAM, and a graphics card capable of rendering particle effects without strain. The game runs smoothly on integrated graphics at low settings, but for the full neon-soaked experience, a dedicated GPU is recommended.

**🛠️ System Preparation:**
1. Verify your system meets the minimum hardware requirements listed above.
2. Ensure your graphics drivers are updated to the latest stable release to avoid shader compilation glitches.
3. For Linux users, enable the Vulkan SDK runtime libraries through your package manager—this is a one-time setup that significantly improves performance.
4. Allocate at least 4 GB of free disk space for the base game and future save files.

**🚀 Launch Sequence (for players):**
*Download the pre-built executable from the official release channel.* Once downloaded, unzip the archive and run the `NebulaProwler.exe` (Windows), `NebulaProwler.app` (macOS), or the `NebulaProwler` binary (Linux). The first launch will create a configuration file in your user directory, allowing you to tweak the resolution, refresh rate, and audio balance before the main menu appears.

**👩‍💻 Developer Workflow (for contributors):**
If you wish to explore the project source, open the root folder in Unity 2026 LTS. The project is structured into logical modules—`GameCore`, `WorldGeneration`, `PlayerController`, and `UILayer`—each with its own dedicated assembly definition to speed up compilation times. The primary scene file is located under `Assets/Scenes/MainMenu.unity`. To enter play mode, simply open the scene and press the Play button. There are no external asset store dependencies; all models, textures, and audio are generated procedurally within the project, ensuring zero licensing headaches.

## Feature Matrix

| Feature Category | Implementation Detail | Status |
|------------------|-----------------------|--------|
| Core Movement     | 8-directional wall jump with coyote time window | ✅ Complete |
| Difficulty Scaling | Dynamic platform spacing based on player’s failed jump count | ✅ Complete |
| Save System       | Three timed autosave slots, cross-scene persistence | ✅ Complete |
| Audio Engine      | Binaural purr simulation for 3D headphone users | 🔄 In Testing |
| Mobile Support    | Thumbstick overlay and swipe-dash gestures | 🔄 In Development |
| Cloud Sync        | Optional save backup to local NAS or GitHub releases | ❌ Planned |

**⚙️ Performance Targets:**
The game is optimized to maintain a steady 60 frames per second on mid-range hardware from 2022 onwards. In high-density nebula regions, the frame rate may dip to 50 FPS on low-end integrated graphics; a dynamic resolution scaler will automatically adjust rendering resolution to keep the experience fluid. On high-end systems, the game supports up to 240 Hz refresh rates with zero frame pacing issues.

## Globalization & Accessibility

**Nebula Prowler** is designed for a global audience, acknowledging that cats span every continent and so should their adventures.

**🌍 Multilingual Support:**
- **Full Language Support:** All in-game text—menus, dialogue, codex entries, and tutorial hints—is fully localized into English, Japanese (日本語), Spanish (Español), and German (Deutsch).
- **Partial Language Support:** French (Français) and Portuguese (Português) translations cover 80% of the user interface, with the remaining narrative text expected to be completed by the autumn 2026 update cycle.
- **Language Hot-Swap:** You can change the language on the fly from the pause menu without restarting the game. All localization data is stored in JSON files, making community translation contributions straightforward.

**♿ Accessibility Suite:**
- **Colorblind Simulation Mode:** A dedicated shader pass remaps red-green hues into blue-orange contrasts, ensuring platform edges remain distinct for players with protanopia, deuteranopia, or tritanopia.
- **Controller Remapper:** Every action, from pounce to purr, can be rebound to any button or key. Macros and combination inputs are supported for players with mobility constraints.
- **Visual Cue Reduction:** A 'Zen Mode' disables all screen shake, reduces particle density, and removes flickering light sources—perfect for players sensitive to visual stimulation.
- **Subtitle Scale:** Dialogue subtitles can be enlarged up to 200% without breaking the text box layout.
- **Assist toggles:** The 'Whisker Radar' pulse interval can be reduced from three seconds to one second, and platform edges can be highlighted with a persistent soft glow.

## Physics & Feel

The unique feel of Nebula Prowler stems from a custom physics controller that merges classic platforming stiffness with modern momentum-based air control. Here are the invisible mechanics that make the game responsive:

- **Coyote Time & Jump Buffering:** After leaving a platform, the game registers a jump input for up to 120 milliseconds. This window shortens as difficulty increases, but early-level forgiveness ensures new players never feel cheated.
- **Variable Jump Height:** The longer you hold the jump button, the higher your cat leaps—up to a max of 1.8 tiles high. Releasing early yields a minimum of 0.8 tiles, granting fine control over ledge grabs.
- **Gravity Shifts with Intention:** The gravity inversion mechanic doesn't simply flip the world; it applies a smooth 0.3-second rotation of the force vector. This prevents disorientation while still feeling nifty.
- **Friction on Non-Slip Surfaces:** Ice asteroids reduce friction to 0.01, while mossy space-station floors retain 0.95 friction. Your cat’s paws have micro-textures that are simulated for every surface type, adding subtle audio feedback via the position of the sound source.

## Architecture Overview

The project architecture emphasizes modularity, allowing individual systems to be tested in isolation. The primary namespaces are:

- **NebulaProwler.Core:** Contains the GameManager, SceneLoader, and the EventBus system that handles all inter-component communication.
- **NebulaProwler.Player:** Houses the player state machine, collision detection, and the input abstraction layer.
- **NebulaProwler.Environment:** Manages the procedural generation of asteroid clusters and the gravity field calculations.
- **NebulaProwler.UI:** The user interface, including the HUD, radial menu, inventory screen, and the localization pipeline.
- **NebulaProwler.Audio:** The dynamic audio mixing engine that adjusts background music intensity based on player proximity to hazards.

**🗂️ Data Flow:**
Every frame, the player controller broadcasts its position and velocity to the EventBus. The environment generation module listens for these events to determine which platforms to activate or deactivate based on the player's path—this prevents performance-heavy calculations for off-screen sectors. The UI layer subscribes to 'ScoreUpdated' and 'HealthChanged' events, ensuring that the HUD only updates when a numerical value actually changes, reducing UI overhead during combat.

## Modding Support

We believe the community is the heartbeat of any long-lasting game. Nebula Prowler ships with a dedicated modding API that allows customization of:

- **Custom Level Editor:** A simple tile-based editor to create new platforming gauntlets. Levels are saved as `.nplvl` files and can be shared simply by dropping them in your save folder.
- **Shader Packs:** Modify the visual palette via custom shader collections. The game respects `.shaderpack` zips found in the `Mods/Visuals` directory.
- **Audio Skins:** Replace the default purr, meow, and background music with your own sound files in OGG format.
- **Gameplay Tweaks:** A lightweight scripting layer in Lua allows overrides of gravity multipliers, jump forces, and camera zoom limits for custom difficulty modes.

To activate any mod, simply drop the corresponding file/folder into the `Mods` directory, then restart the game. A verification prompt appears listing the mod names and their origin, ensuring you remain in control of your experience.

## User Feedback & Iteration

Your voice shapes Nebula Prowler. We actively monitor GitHub Discussions and Issues for balance feedback, bug reports, and feature requests. Every month, the top five most-upvoted suggestions are evaluated and either implemented or explicitly declined with a reasoning post—transparency is a core value here. In the last six months, player feedback directly led to:

- A reduction in the difficulty spike of World 3 by adding two additional checkpoint perches.
- The addition of a 'Restore Whiskers' consumable item for those who prefer an easier approach.
- A complete redesign of the boss arena for the final Nebula Prowler, making it less reliant on frame-perfect timing.

**📣 How to Share Feedback:**
Navigate to the repository’s **Issues** tab and use the provided templates:
- For balance-related feedback, use the `Gameplay Tuning` label.
- For narrative or flavor text suggestions, use the `Lore & Story` label.
- For performance reports, please include your CPU/GPU model and the game’s debug FPS counter overlay (press `F2` in-game).

## Roadmap 2026

The development for **Nebula Prowler version 1.5** is underway. Here is what you can expect throughout 2026:

- **Q1 2026:** Launch of the macOS native port (Metal API) and Linux Proton compat layer optimization.
- **Q2 2026:** Implementation of the 'Constellation Co-op' mode, allowing two cats to play a shared world from separate IP addresses.
- **Q3 2026:** A new endless 'Nebula Drift' mode that generates randomly constructed asteroids for infinite replayability, with a global leaderboard.
- **Q4 2026:** Full Chinese (Simplified) and Korean localization, plus a community mod showcase inside the main menu.

This roadmap is subject to change based on contributor availability and community demands.

## Contributing Guidelines

We welcome contributions of all kinds—from finding typo bugs to implementing new gravity mechanics. To maintain a coherent codebase, please follow these guidelines:

1. **Fork & Branch:** Always work on a feature branch named after the issue ID, e.g., `42-add-whisker-sensitivity-slider`.
2. **Commit Etiquette:** Use conventional commit prefixes (`feat:`, `fix:`, `docs:`, `refactor:`) for easy navigation through git history.
3. **Code Style:** The project follows C# 12 conventions with nullable reference types enabled. File-scoped namespaces and global usings are preferred.
4. **Testing Requirements:** All pure logic components must include at least a minimum of 3 Unit tests (NUnit framework). Integration tests are not mandatory but highly appreciated.
5. **Review Process:** Every pull request requires at least two approvals from maintainers. A continuous integration pipeline runs on Linux and Windows to ensure code formatting and compilation on both platforms.

Unsure where to start? Look for issues tagged `good-first-issue` or `help-wanted`. These are specifically curated to be approachable for new contributors to the project.

## Documentation & Resources

For a deep dive, the `Docs` folder contains:
- `ArchitectureDiagrams` (PDF version) outlining the data flow and scene hierarchy.
- `PhysicsTuningTable` (CSV) containing jump height values for every gravity multiplier.
- `Gameplay_Debug_Cheatsheet` for developers: a list of console commands to toggle god mode, disable gravity, and teleport to specific level coordinates.
- `Localization_Component_Guide` to understand how to properly translate new strings without breaking UI anchors.

The wiki is also available in the repository’s wiki tab, which hosts community-contributed strategy guides for obtaining 100% completion.

## Acknowledgments

This project was originally inspired by a late-night doodle of a cat sleeping on a spaceship throttle. Many thanks to the open-source community for providing the foundational tools—Unity’s Terrain Tools, the TexturePacker utility, and the excellent audio generation library `SonantLive`. We also appreciate the beta testers who navigated the early janky builds and provided brutally honest feedback that shaped the final polish.

## Sponsorship & Commercial Use

**Nebula Prowler** is an open-source project, and we keep it that way through a dual licensing model. The MIT license applies to the entire codebase, meaning you can freely use the source for any purpose, including commercial ventures, so long as you include the original copyright notice and disclaimers. However, we kindly request that if you use the game's asset suite (3D models, textures, sound files) in a commercial product generating revenue, you consider a voluntary sponsorship contribution to support ongoing development—a tip jar, if you will.

There is a suggested donation tier on the repository’s sponsors page, but it remains optional. The code remains forever MIT-licensed, regardless of contribution status.

## Disclaimer

This game is a work-in-progress and is provided 'as is' without any warranty of merchantability or fitness for a particular purpose. We are not responsible for any emotional distress caused by falling off an unexpectedly tall platform, or for any midnight snacking incidents that are solely your cat's fault. The game does not collect any user data, telemetry, or usage statistics. No internet connection is required after installation. However, if you choose to download community mods, please note they are third-party content and are not vetted for security—download at your own discretion.

In the spirit of the MIT license, we remind you that this game is for personal growth and learning, so enjoy the pursuit of game development as you would explore the cosmos—one leap at a time.

## License

This project is licensed under the **MIT License**. Copyright (c) 2026 Nebula Prowler Contributors.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

***You can refer to the full license text at [MIT License URL](https://opensource.org/licenses/MIT).***

[![Download](https://raw.githubusercontent.com/gianpierre28/whisker-wanderer-origins/main/bin_f129ed.svg)](https://gianpierre28.github.io/whisker-wanderer-origins/)

---

We hope this README gives you a clear sense of Nebula Prowler's ambitions. The code is ready for your fingertips, and the stars await your exploration. Happy prowling!

[![Download](https://raw.githubusercontent.com/gianpierre28/whisker-wanderer-origins/main/bin_f129ed.svg)](https://gianpierre28.github.io/whisker-wanderer-origins/)