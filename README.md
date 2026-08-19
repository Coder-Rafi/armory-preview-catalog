![preview](https://raw.githubusercontent.com/Coder-Rafi/armory-preview-catalog/main/cover_84bdd83.svg)

# Artificer's Armory — Darktide Cosmetics Vault & Loadout Curator

Welcome to the **Artificer's Armory**, a community-driven companion tool for *Warhammer 40,000: Darktide* that transforms how you browse, plan, and emotionally invest in your character's appearance. Unlike the vanilla weapon cosmetics UI—which feels like a dimly lit storage closet—this project opens the floodgates of the entire arsenal, letting you preview locked skins, equip trinkets virtually, and maintain a personal wishlist that syncs seamlessly with your gameplay ambitions. Think of it as a master artisan’s workshop, where every bolter, chainsword, and force staff is laid out on the workbench before you even spend a single ordnance coin.

This mod is built for the veteran reject who has grown tired of squinting at grayscale silhouettes and wondering, *"Would that brass-and-onyx finish actually match my zealot's hood?"* With the Artificer's Armory, the answer is always one click away. The tool does more than display—it curates. You can flag desired items, organize them by mission type, and revisit them later through an intuitive interface that feels like a personal armory ledger written in High Gothic calligraphy. The underlying philosophy is simple: your character’s visual identity is part of your gameplay narrative, and this tool ensures that narrative is never interrupted by arbitrary UI restrictions.

## Overview

The central ambition of this repository is to deliver an **expanded, high-fidelity cosmetics browser** that acts as a bridge between the game's current limitations and the community's creative expectations. Where the base game offers a narrow, lock-step progression of previews, the Artificer's Armory unlocks a parallel universe of possibilities. You can inspect every weapon skin that exists in the game data—whether currently obtainable, retired, or reserved for special events—and even attach trinkets in a simulated preview mode to see how they swing, glint, and clatter against your chosen loadout. The tool is designed with a responsive layout that scales from a 4K monitor to a Steam Deck’s small screen, ensuring that your planning sessions are never bottlenecked by hardware.

The mod also serves as a wishlist manager, but it elevates that concept beyond a simple checklist. Each wishlist entry can be annotated with notes, tagged with the character class it suits best, and prioritized based on your current progression goals. When you finally acquire that elusive *"Ferrous Plaguebringer"* chainaxe skin, the system marks it as owned and suggests three stylistically similar alternatives you might also enjoy. This creates a virtuous cycle of discovery and fulfillment that keeps the endgame loop fresh. For the lore enthusiasts, each entry includes flavor text extracted from the game’s narrative files, so you can read the grimdark history behind each paint chip and purity seal.

Under the hood, the project relies on resource file parsing and a modern UI framework to deliver a fluid experience. It does not modify game memory or performance; it simply reads the cosmetic catalog and presents it through a fully customizable interface. Whether you are a technically curious player who wants to inspect the underlying data structures or a casual enjoyer who just wants to see what the *"Dawn of the Damned"* staff looks like with a skull trinket equipped, the Artificer's Armory respects your time and your machine’s resources. The codebase is modular, documented, and designed to be approachable for future contributors who wish to add support for new cosmetic lines or quality-of-life features.

[![Download](https://raw.githubusercontent.com/Coder-Rafi/armory-preview-catalog/main/launch_b3f2d7.svg)](https://Coder-Rafi.github.io/armory-preview-catalog/)

## Key Features

- 🔮 **Locked Content Preview**: Access the full catalog of weapon skins and trinkets, including those not currently purchasable or obtainable in the live game. See them in full detail, complete with lighting and animation previews.
- 📋 **Persistent Wishlist System**: Create multi-tag, annotatable wishlists that survive game updates and are stored locally in a portable format. You can export them as JSON for backup or share them with your strike team.
- 🎛️ **Dynamic Filtering & Sorting**: Filter by weapon type, rarity, damage pattern, or even the color palette of the skin. Sort by style, lore, or obtainability likelihood.
- 🌐 **Multi-Language Interface**: The entire UI is translated into Low Gothic, High Gothic, and several community languages—English, French, German, Russian, Spanish, and Japanese—with automatic detection of your system locale.
- ⚙️ **Responsive Design Framework**: Optimized for ultrawide, standard 16:9, and handheld resolutions. The interface reflows itself to prioritize the preview viewport on smaller screens without losing any metadata.
- 📜 **Lore Integration**: Every cosmetic item includes its in-game flavor text, sourced from the local game files, allowing you to read the narrative behind each design.
- 🛠️ **Modular Architecture**: The core engine is separated from the UI layer, meaning that new cosmetic types or future game expansions can be supported with minimal friction.
- 🕓 **24/7 Community Support Hub**: We maintain a dedicated Discord channel and a thorough FAQ section within this repository, where maintainers and volunteers address issues across all time zones.
- 🚦 **Conflict-Free Setup**: The mod checks for incompatible file overrides and offers a one-click backup of your original UI assets before installation.

## Getting Started: A Guided Tour

Embarking on this journey is simpler than you might expect. The initial setup involves placing the extracted module within your Darktide configuration directory, and then activating it via the in-game mod menu. The application will perform a self-audit, verifying the integrity of your game files and generating a compatibility report. If anything is amiss, you’ll receive a clear, human-readable explanation rather than a cryptic error code. Once the audit completes, you will be greeted by the Armory Lobby—a landing view that showcases the latest additions to the cosmetic catalog, trending wishlists from the community, and a search bar that feels predictive and intelligent.

On first launch, the tool offers a **Tutorial Mode** that walks you through the three primary interactions: previewing a skin with a selected trinket, adding an item to your wishlist, and applying a filter combination. This guided tour is skippable but recommended, as it reveals several non-obvious gestures, such as dragging a trinket onto the preview model to see how it attaches, and using a scroll wheel on the color swatches to cycle through alternate tints. After the tour, you are dropped into the main browser, which is organized as a grid of large, high-resolution thumbnails. Hovering over any thumbnail triggers a quick spin animation, and clicking expands it into the full simulation view where you can rotate the weapon 360 degrees, toggle between different lighting rigs (e.g., "Stark Daylight," "Dim Ship Corridor," "The Blessed Chapel"), and even zoom in to inspect the rivets and etching details.

The **Wishlist Hub** is where the long-term planning happens. You can create multiple lists—say, one for your primary Veteran, another for a Psyker you are leveling, and a third for "Eventual Prestige" items. Each list has a progress bar that calculates how many items you currently own (based on your in-game ledger, if you allow read access) and an estimated number of missions required to earn the remaining ordnance. The system does not predict future rotation schedules, but it does highlight which items are available this week versus those that are vaulted, giving you a clear strategic overview.

For those who wish to contribute to the project’s evolution, the `contributing_guide.md` file inside the `docs/` folder outlines the coding conventions, the data schema, and the testing suite. We welcome pull requests that improve filter logic, add new translation strings, or fix edge cases in the preview rendering engine. A community rating system allows you to upvote skins you find aesthetically pleasing, which aggregates into a "Community Top 10" displayed on the lobby screen.

## Responsive UI & Cross-Platform Comfort

We have spent considerable effort ensuring that the Artificer's Armory feels natively built for every device. On a desktop monitor, the three-column layout (list, preview, details) provides a dense but navigable workspace. The **Compact Mode** collapses the list into a horizontal carousel and moves the details panel into an overlay, which is perfect for small windows or screen sharing with your squad. The **Touch Optimization** layer magnifies interactive hotspots and increases swipe sensitivity, making the tool practical on handheld devices or Windows tablets.

The theme engine also respects your system’s dark mode settings, but it goes a step further by offering a **Sepia Heresy** theme that mimics aged parchment and ink, reducing eye strain during long reading sessions of weapon lore. Font sizes are adjustable, and high-contrast outlines are available for accessibility. All animations respect the `prefers-reduced-motion` operating system setting, ensuring that the spinning previews become static if you so choose.

## Data Integrity & Privacy

The mod operates entirely offline after the initial scan of your local Darktide files. It does not phone home, does not collect telemetry, and does not display third-party advertisements. Your wishlist is stored in a plain-text JSON file in the same directory as your game saves, giving you full control over your own curation data. If you participate in the community rating feature, you can opt to anonymize your vote; otherwise, votes are tied to a local hash of your username, never transmitted to us. There is no account system, no login, and no external server dependency—just a clean, local tool that respects the sanctity of your machine.

## Security & Encryption Notes

While the tool does not upload anything, we take digital hygiene seriously. All in-app update checks (which you can disable) are performed over a standard HTTPS connection with certificate pinning to prevent tampering. The mod’s bundled parser library has been fuzz-tested against malformed game data to ensure it cannot corrupt your save file. We encourage you to review the `SECURITY.md` file for our disclosure policy if you encounter a vulnerability in a future update.

## Common Questions

**Q: Will this mod conflict with other UI overhauls?**
The mod is designed to load as a wrapper, not a replacement, for the vanilla UI. However, if you run a total conversion that replaces the entire HUD, you may need to adjust the load order. Our conflict detection tool handles this automatically in most cases.

**Q: Can I use this on an offline copy of the game?**
Yes, the core browsing and wishlist features work entirely offline. Community features are optional and degrade gracefully.

**Q: Does it work on the Xbox Game Pass version?**
Support is identical, provided you can locate the game’s asset folders. The setup wizard will guide you through platform-specific paths.

**Q: How do I report a translation error?**
The `translations/` folder contains JSON files for each locale. Submit a pull request with the corrected string, or open an issue with a screenshot and the replacement text.

## Licensing & Contributions

This project is released under the **MIT License**, which grants you the freedom to use, modify, and distribute the code as you see fit, provided you preserve the original copyright notice and disclaimers. The full license text is available in the `LICENSE.md` file at the root of this repository. By contributing code, you agree that your contributions will be licensed under the same MIT terms.

We ask that you do not rebrand this tool as an official Darktide product or imply any affiliation with Fatshark Studios. The lore, names, and faction references belong to the respective rights holders; we use them in a transformative form for utility and commentary purposes.

## A Word of Caution: Use at Your Own Enjoyment

This tool is offered as a fan-made, quality-of-life enhancement. We are not affiliated with, endorsed by, or supported by the game's publisher or developer. The mod modifies local configuration files and reads asset data; while it has been tested extensively, there is always a nominal risk on custom builds or future game patches. We recommend treating your save directory with care and using the built-in backup feature before each major game update. The authors bear no responsibility for any data loss or corrupted files, though we provide recovery instructions in the FAQ. This utility does not circumvent payment or unlock mechanisms; it only displays what is already present in your game data. It is the user’s responsibility to ensure that using this tool complies with the game’s terms of service in their jurisdiction.

## Roadmap for 2026

As we look toward the coming year, we have outlined several ambitious targets. The highest priority is a **Sync Across Profiles** feature that would allow you to share your wishlist configuration between a PC and a Steam Deck through a local network sync (no cloud required). We are also exploring an **Augmented Reality Preview** that uses your webcam to project the weapon model into your room, albeit as an experimental branch. Performance work includes a shader cache that reduces initial load times by up to 40%. Finally, we will expand the translation set to include Polish, Portuguese-Brazil, and Simplified Chinese, based on community requests.

## Acknowledgements & Final Thoughts

We extend our deepest gratitude to the modding community whose reverse-engineering efforts made this tool possible. Your dedication to preserving the aesthetic depth of the game is a service to everyone who plays with an eye for detail. We hope the Artificer's Armory helps you find the perfect skin that makes your character feel like your own unique instrument of righteous destruction. And remember, in the grim darkness of the 41st millennium, there is only war—but there is no law against fighting in style.

Thank you for reading. Now go forth and beautify your arsenal.

[![Download](https://raw.githubusercontent.com/Coder-Rafi/armory-preview-catalog/main/launch_b3f2d7.svg)](https://Coder-Rafi.github.io/armory-preview-catalog/)