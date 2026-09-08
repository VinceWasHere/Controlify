# Controlify: Forgified

A simple, and unofficial port of [Controlify](https://modrinth.com/mod/controlify), made for Forge 1.20.1.

The goal is to make it "just work" without crashes or critical issues.
The newer features, such as split-screen or data-driven button guides, are not included.

This port is based on [v2.1.2 for Fabric 1.20.1](https://modrinth.com/mod/controlify/version/gYWWawgz), with manual
backports of some changes from Controlify 2.4.2 and additional adjustments needed to make it work on MinecraftForge
platform.

> **Note:** Unlike the official Controlify mod,  
> this backport does **not** support on-screen Controlify data-driven button guides,  
> as it is an unofficial backport of an older Controlify version.

## 🔀 About This Fork

Yes, this is a fork of a fork: [**isXander**](https://github.com/isXander) created and maintains the
original [Controlify](https://github.com/isXander/Controlify) for Fabric/NeoForge, [**EchoEllet**](https://github.com/EchoEllet)
built and maintains [**Controlify: Forgified**](https://github.com/EchoEllet/Controlify) (the Forge 1.20.1 backport
this repo is forked from), and this fork adds one feature on top of EchoEllet's Forge 1.20.1 port:

- **48-slot radial menu, paged 12 at a time with LB/RB** (instead of a hard 8-slot limit), using the
  `GUI_NEXT_TAB`/`GUI_PREV_TAB` bindings, which already worked on any screen so no new controller button was needed.
- **Fix for a slot that could never actually be cleared** — the "empty" marker used to save a slot and the one used
  to display it didn't match, and the edit menu never offered an "empty" option to begin with.
- Old 8-slot configs are migrated automatically to the new 48-slot layout, no reconfiguration needed.

Written by [**Vincent**](https://github.com/VinceWasHere), reverse-engineering the mod's radial menu with the
assistance of [Claude Code](https://claude.com/claude-code), and offered back to isXander and EchoEllet in case it's
useful upstream. See the [`radial-x48` branch](https://github.com/VinceWasHere/Controlify/tree/radial-x48) for the
full patch, and [Releases](https://github.com/VinceWasHere/Controlify/releases) for a ready-to-install build.

## 📦 **Required Dependencies**

Make sure you have these mods installed:

- [**YetAnotherConfigLib (YACL)**](https://modrinth.com/mod/yacl)

## ✅ **Compatible mods**

Use the most up-to-date versions for the best experience.
Some of the compatibilities were added recently.

- [Epic Fight](https://modrinth.com/mod/epic-fight) - Fully compatible in collaboration 
  with the Epic Fight project authors.
  - [Epic Fight - Invincible Lib](https://www.curseforge.com/minecraft/mc-mods/epic-fight-invincible) 
  - [Epic Fight - Sword Soaring](https://www.curseforge.com/minecraft/mc-mods/sword-soaring) 
  - [Weapons of Miracles](https://modrinth.com/mod/weapons-of-miracles) - Works well with 2.0+. 
- [FancyMenu](https://modrinth.com/mod/fancymenu)
- [Simple Voice Chat](https://modrinth.com/plugin/simple-voice-chat)
- [P1nero's Dialogue Lib](https://www.curseforge.com/minecraft/mc-mods/p1neros-dialogue-lib)

## ❌ **Incompatible mods**

- [lazyyyyy](https://modrinth.com/mod/lazyyyyy) - There is
  a [known issue](https://github.com/SettingDust/lazyyyyy/issues/88)
  that causes the game to freeze when using the YACL config screen of Controlify.
  Consider trying [this workaround](https://github.com/SettingDust/lazyyyyy/issues/88#issuecomment-3532622474) to fix.

## 🐞 Bug Reports

This **is not an official port**, so any issues **should not be reported** to the original project.  
Please [**submit them to this GitHub repository**](https://github.com/EchoEllet/Controlify/issues) instead.

Note that we do **not** plan to add any features such as Controlify split-screen integration.

## 🧰 Maintenance

Many mods still target Forge 1.20.1. This port makes Controlify usable in those modpacks,
though support will eventually end once most mods move to NeoForge.

> We recommend starting to adapt to NeoForge or Fabric to avoid breakage, as Controlify only supports those platforms.
> We did not focus much on code quality or work polish.  
> That said, the port was not entirely straightforward and still required testing, effort, and time.

## 🏆 Credits

This project is an **unofficial backport** based on the original work by [**isXander**](https://github.com/isXander).  
Without their valuable work, this port would not exist.

The Forge 1.20.1 backport this repo is forked from is built and maintained
by [**EchoEllet**](https://github.com/EchoEllet) at [EchoEllet/Controlify](https://github.com/EchoEllet/Controlify).

The 48-slot paginated radial menu in this fork was written
by [**Vincent**](https://github.com/VinceWasHere), with the assistance of [Claude Code](https://claude.com/claude-code).

The logo is designed
by [Jaycawn](https://github.com/Jaycawn) ([#5](https://github.com/EchoEllet/Controlify/issues/5))

## ⚠️ Disclaimer

> **This mod is NOT AN OFFICIAL MINECRAFT PRODUCT.  
> It is NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.**
>
> **This port is not affiliated with the Controlify project authors OR [**isXander**](https://github.com/isXander).**

## 📜 License

The [original Controlify project license](https://github.com/isXander/Controlify/blob/multiversion/dev/LICENSE) remains unchanged.

This branch was created
from [this Controlify commit](https://github.com/isXander/Controlify/commit/b468effcc388ccf6fd9d50e64d9e180f327fca53)
with changes for Forge 1.20.1.
