# Controlify: Forgified — Vincent's fork

This is [**Vincent**](https://github.com/VinceWasHere)'s fork of [**EchoEllet's Controlify: Forgified**](https://github.com/EchoEllet/Controlify)
(an unofficial backport of [**isXander**](https://github.com/isXander)'s [Controlify](https://github.com/isXander/Controlify)
to Forge 1.20.1). **This default branch is an unmodified copy of EchoEllet's `1.20.1-forge` branch** — none of the
code below is Vincent's. It's kept here only so this fork can track upstream normally.

The actual reason this fork exists — a 48-slot, paginated radial menu — lives on the
[**`radial-x48` branch**](https://github.com/VinceWasHere/Controlify/tree/radial-x48), with a ready-to-install
build in [**Releases**](https://github.com/VinceWasHere/Controlify/releases). Go there, not here, if you want
what this fork actually adds.

## ⚠️ About the radial-x48 patch

It was written by reverse-engineering the compiled mod and porting the result onto EchoEllet's source, with the
help of [Claude Code](https://claude.com/claude-code). It's been tested by hand with a real and virtual gamepad,
but has **not** been reviewed by isXander or EchoEllet and is **not** an official release of either project. It
may contain bugs the manual testing missed. Report issues with it on
[this fork's issues](https://github.com/VinceWasHere/Controlify/issues), not on EchoEllet's or isXander's repos.

## 🏆 Credits

- [**isXander**](https://github.com/isXander) — created and maintains the
  original [Controlify](https://github.com/isXander/Controlify).
- [**EchoEllet**](https://github.com/EchoEllet) — built and maintains
  [**Controlify: Forgified**](https://github.com/EchoEllet/Controlify), the Forge 1.20.1 backport this fork is
  based on, and everything on this branch.
- [**Vincent**](https://github.com/VinceWasHere) — the radial x48 patch (on the `radial-x48` branch), with the
  assistance of [Claude Code](https://claude.com/claude-code).
- [**Jaycawn**](https://github.com/Jaycawn) — designed the mod logo
  ([EchoEllet/Controlify#5](https://github.com/EchoEllet/Controlify/issues/5)).

---

Everything from here down is EchoEllet's original README, unchanged, because it still describes this branch
exactly as EchoEllet wrote it.

A simple, and unofficial port of [Controlify](https://modrinth.com/mod/controlify), made for Forge 1.20.1.

The goal is to make it "just work" without crashes or critical issues.
The newer features, such as split-screen or data-driven button guides, are not included.

This port is based on [v2.1.2 for Fabric 1.20.1](https://modrinth.com/mod/controlify/version/gYWWawgz), with manual
backports of some changes from Controlify 2.4.2 and additional adjustments needed to make it work on MinecraftForge
platform.

> **Note:** Unlike the official Controlify mod,  
> this backport does **not** support on-screen Controlify data-driven button guides,  
> as it is an unofficial backport of an older Controlify version.

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
Please [**submit them to EchoEllet's repository**](https://github.com/EchoEllet/Controlify/issues) instead
(or to [this fork's issues](https://github.com/VinceWasHere/Controlify/issues) if the bug is specific to the
radial-x48 patch).

Note that we do **not** plan to add any features such as Controlify split-screen integration.

## 🧰 Maintenance

Many mods still target Forge 1.20.1. This port makes Controlify usable in those modpacks,
though support will eventually end once most mods move to NeoForge.

> We recommend starting to adapt to NeoForge or Fabric to avoid breakage, as Controlify only supports those platforms.
> We did not focus much on code quality or work polish.  
> That said, the port was not entirely straightforward and still required testing, effort, and time.

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
