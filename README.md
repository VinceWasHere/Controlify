# Controlify: Forgified — Radial x48

This is [**Vincent**](https://github.com/VinceWasHere)'s fork of [**EchoEllet's Controlify: Forgified**](https://github.com/EchoEllet/Controlify)
(itself an unofficial backport of [**isXander**](https://github.com/isXander)'s [Controlify](https://github.com/isXander/Controlify)
to Forge 1.20.1). The only thing this fork adds is a bigger, paginated radial menu — everything else is
EchoEllet's port, unchanged.

## ⚠️ Made with AI assistance — read before installing

This fork's patch was written by reverse-engineering the compiled mod and porting the result onto EchoEllet's
source, with the help of [Claude Code](https://claude.com/claude-code). It has been tested by hand with a
real and virtual gamepad, but it has **not** been reviewed by isXander or EchoEllet, and it is **not** an
official release of either project. It may contain bugs that the manual testing missed. Use at your own risk,
and please [open an issue on this fork](https://github.com/VinceWasHere/Controlify/issues) — not on EchoEllet's
or isXander's repositories — if you run into problems with this specific patch.

## 🔀 What this fork changes

- **48 radial slots instead of 8**, shown 12 at a time and paged with `LB`/`RB`
  (`GUI_PREV_TAB`/`GUI_NEXT_TAB`, which already worked on any screen, so no new controller button was needed).
- **Fixed a slot that could never actually be cleared** — the "empty" marker used to save a slot and the one
  used to display it didn't match, and the edit menu never offered an "empty" option to begin with.
- Old 8-slot configs are **migrated automatically** to the new 48-slot layout — no reconfiguration needed.

Source diff: [`radial-x48` branch](https://github.com/VinceWasHere/Controlify/tree/radial-x48).
Ready-to-install build: [Releases](https://github.com/VinceWasHere/Controlify/releases).

## 🏆 Credits

- [**isXander**](https://github.com/isXander) — created and maintains the
  original [Controlify](https://github.com/isXander/Controlify). Without their work, none of this would exist.
- [**EchoEllet**](https://github.com/EchoEllet) — built and maintains
  [**Controlify: Forgified**](https://github.com/EchoEllet/Controlify), the Forge 1.20.1 backport this fork is
  based on. All of the sections below this point describe EchoEllet's work, reproduced here because they still
  apply unchanged to this build.
- [**Vincent**](https://github.com/VinceWasHere) — wrote the radial x48 patch in this fork, with the
  assistance of [Claude Code](https://claude.com/claude-code).
- [**Jaycawn**](https://github.com/Jaycawn) — designed the mod logo
  ([EchoEllet/Controlify#5](https://github.com/EchoEllet/Controlify/issues/5)).

---

The following sections are EchoEllet's, from [Controlify: Forgified](https://github.com/EchoEllet/Controlify),
reproduced here because they describe the mod this fork is built on and still apply as-is.

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

For issues with the base Controlify: Forgified port, please use
[EchoEllet's repository](https://github.com/EchoEllet/Controlify/issues) — not the original Controlify project.
For issues specific to the radial x48 patch in this fork, use
[this repository's issues](https://github.com/VinceWasHere/Controlify/issues) instead.

## 🧰 Maintenance

Many mods still target Forge 1.20.1. This port makes Controlify usable in those modpacks,
though support will eventually end once most mods move to NeoForge.

> We recommend starting to adapt to NeoForge or Fabric to avoid breakage, as Controlify only supports those platforms.

## ⚠️ Disclaimer

> **This mod is NOT AN OFFICIAL MINECRAFT PRODUCT.  
> It is NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.**
>
> **This fork is not affiliated with the Controlify project authors, EchoEllet, OR [**isXander**](https://github.com/isXander).**

## 📜 License

The [original Controlify project license](https://github.com/isXander/Controlify/blob/multiversion/dev/LICENSE) remains unchanged.

This branch was created
from [this Controlify commit](https://github.com/isXander/Controlify/commit/b468effcc388ccf6fd9d50e64d9e180f327fca53)
with changes for Forge 1.20.1, forked from [EchoEllet/Controlify](https://github.com/EchoEllet/Controlify).
