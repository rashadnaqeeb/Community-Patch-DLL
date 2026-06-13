# Modification Notice

This repository is a modified fork of the Community Patch DLL (Vox Populi),
originally developed by the Community Patch Project (LoneGazebo and
contributors): https://github.com/LoneGazebo/Community-Patch-DLL

The upstream work is licensed under the GNU General Public License v3 (see
`License.rtf`). This fork is distributed under the same license. All upstream
copyright and license notices are preserved unchanged.

## What this fork changes

This fork exists to support Civ V Access, an accessibility layer that makes
Sid Meier's Civilization V playable for blind players. On top of the upstream
`Release-5.3.2` tag, the `civvaccess` branch adds:

- Lua bindings the accessibility mod relies on: the unit mission queue,
  build-route and pathfinder helpers, league member-detail strings, and
  extended arity on the best-defender and move-or-attack bindings.
- Engine event hooks the mod listens on for live speech output (mission
  dispatch, unit movement, plot reveal, goody/barb-camp, combat resolution,
  nukes, air sweep).
- Player-set trade unit names carried across the engine's trade-unit respawns
  so nicknames survive a route's lifecycle.
- Build-script fixes for compiling the DLL under newer Python and the
  clang/LLVM toolchain.

Modified source files carry inline `CIVVACCESS:` comments marking each change.
These modifications were made in June 2026 by Rashad Naqeeb.

The Community Patch Project is not affiliated with, and does not endorse, this
fork.
