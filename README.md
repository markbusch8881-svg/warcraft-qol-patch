# Warcraft: Orcs & Humans — quality of life patch

Four small changes to the original 1994 DOS game.

## What it changes

- **Right-click gives an order** instead of scrolling the view. Units walk to open
  ground, attack an enemy, send a peasant or peon to a gold mine, carry a load back to
  the town hall, repair one of your own buildings, or chop forest.
- **Right-click works on the minimap** too, with the same orders. Left-click still
  moves your view there.
- **The map scrolls at the screen edge** when the pointer reaches it, no click needed.
- **Water and the building outline animate at a steady speed.** Both used to run
  faster on a faster machine.

Known limitation: select a mixed group, say a peasant and a footman, and they all move
rather than each doing the sensible thing for its type. Orders go to the group as a
whole.

## What you need

- **Warcraft: Orcs & Humans, CD release, version 1.22h.** Your `war.exe` must be
  319,291 bytes with SHA-256
  `1e966220bf09ab007c49c5ea5ebc42eb494f5cf2f74f894d3969b6115df8d8a9`. The patch checks
  this and refuses anything else, so the floppy release and other versions will not
  work.
- **Flips**, from
  [romhacking.net/utilities/1040](https://www.romhacking.net/utilities/1040/).
  Windows, Linux and macOS.

The patch holds only the bytes that differ from the original, so you supply the game.

## Applying it

1. Make a **copy** of your `war.exe` somewhere convenient, and leave the original
   where it is so you can go back to it.
2. Run Flips and choose **Apply patch**. Pick `warcraft-gameplay.bps`.
3. Pick your copy of `war.exe`, then choose where to save the result — call it
   `war-patched.exe`.
4. Put `war-patched.exe` in your Warcraft folder and run it instead of `war.exe`,
   however you normally start the game.

## If Flips refuses

**"This patch is not intended for this ROM. Expected checksum A3EE9116, got ..."**

Your `war.exe` is not CD v1.22h. Usually the floppy release, a different version, a
copy an installer changed, or one you already patched — start from a fresh copy.
Nothing was written. Flips calls your `war.exe` a ROM, which is just how it words it.
