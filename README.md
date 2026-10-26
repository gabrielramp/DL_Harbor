
<img width="1606" height="401" alt="banner_03" src="https://github.com/user-attachments/assets/e4c0cd53-dc82-4b57-9528-4735fe361781" />

<h1 align="center">dl_harbor</h1>

<p align="center"><a href="../../releases"><b>Download from the Releases page</b></a></p>

Hello! Thank you for taking the time to play dl_harbor!

dl_harbor is a 4v4, two-lane Deadlock map focused on a bigger economy, snowballing fights, impactful plays and dynamic events.

### Installation

1. Download `Client-Setup.exe` from the [Releases page](../../releases) and run it.
2. When it asks, point it at your `Deadlock.exe` (inside `steamapps\common\Deadlock\game\bin\win64\`).

The setup installs the map and its addon for you. To install by hand instead, place `dl_harbor.vpk` in
`steamapps\common\Deadlock\game\citadel\maps\`.

That's it!

### Playing

- It is **strongly recommended** to play on a [Deadworks](https://docs.deadworks.net/getting-started/server-admins/run-a-server) server. Many abilities, interactions and more can and will break without one.
- To just run around the map: open the console (F7), type `map dl_harbor` and press Enter.

### Hosting a server

Use `Server-Setup.exe` from the [Releases page](../../releases). It installs the Harbor server plugin with the game settings crafted for the intended experience, the map, and the addon, and adds `harbor` to your server's content addons.

Then update your `run-server.bat` so the server launches into `dl_harbor`.

#### Settings

The plugin reads `harbor-balance.yaml` from `game\bin\win64\managed\plugins\`, next to `harbor-plugin.dll`. Edit it and restart the server to change a value; each key names its unit. A file with a typo or a missing key is refused as a whole: the server runs stock Deadlock and logs one `[Harbor] settings NOT applied` line naming the problem.

> **Upgrading?** The setup never overwrites an existing `harbor-balance.yaml`, so your edits survive a reinstall. When a release adds settings, copy the new sections from the release's `harbor-balance.yaml` into yours. v2.3 adds `zipline_boost` and `rejuvenator_crystal`.

### Features

- **Two lanes:** an upper lane (Bank) and a lower lane (Harbor).
- **The Broker has arrived at the harbor!**
- **Vaults:** a central lighthouse illuminates a vault. One minute later the ethereal hand descends and the vault opens, revealing a large number of souls to claim and fight over.
- **Increased economy:** faster camp respawns, more trooper value, a surplus of crates, faster crate and idol respawns, and soul vaults.
- **Earned movement:** as your team kills guardians and walkers, it gains boost pads towards the enemy.
- **Custom art.**

### Known issues

- Midtown's minimap is shown instead of Harbor's.
- Shop locations can be inaccurate on the minimap, mainly at the HK blue guardian.
- Troopers sometimes bypass the shrines and gather around the patron.
- Lane ziplines do not stay neutral at the start of the game.

### Community

Join the dl_harbor Discord to give feedback or play in hosted games!

Cheers and happy vaulting.
— Scott "Seismic"

### Updates

#### v2.3

- Custom installers: one for the map, one for servers (thank you to @jetsetworm for the help).
- Major art changes in front of Archmother.
- Major art changes for blue lane walkers.
- Layout changes in the secret shop tunnels.
- Added steam vents.
- Clipping, lighting and performance updates.

**Modified values**

- More souls from all sources.
- Crates now drop 75% of the time (from 60%).
- Golden Idols now drop 75% of the time (from 50%).
- Midboss health is 60% of original.
- Zipline boost cooldown is now 50% of original (3 min instead of 6 min).
- The Rejuvenator crystal now breaks after 2 hits (from 3), so it can be claimed twice.
- The Broker now appears at 15 min, and again at 25 min (to help close out the game).
- "Vault will open soon" announcement added.
- Global sound added for the vault opening.
- Troopers spawn quicker starting at 5 minutes.
- Spectators in free camera now see HUD announcements (vaults, the Broker and more).

#### v2.2 — City Never Sleeps compatibility

Updated to City Never Sleeps:

- Updated camps.
- Added strong boxes.
- Pings, drawing and Mirage's ultimate are fixed!
- The Urn now starts on the upper (yellow) lane.
- The ship vault is now on the upper deck instead of in the veil.
- Fixed the ship vault's vase spawn offset.

**Secret Shop**

- Opened up the cellar room foyer.
- Removed two pillars in the Secret Shop.
- Clipping fixes (a lot). Some standouts: Bank lane, the phone booth, holes in the ceiling of the level.
- Fixed stairs that killed your momentum on the buff building and the Archmother mystic roof.
- Moved odd boxes on HK blue lane.
- Barracks Guardians are now themed appropriately.
- Added a handful of extra boxes across the map.
- HK yellow lane camp now respawns when cleared.
- AM blue lane camp now respawns when cleared.
- Lowered shrine health from 2500 to 1800.
- Lightmap fixes.

**General layout and art**

- Lowered the upper ground at the blue lane walkers (HK and AM).
- Outdoor climb ropes are now held aloft by a mystic hand.
- Added a handful of street signs to help direct players.
- Turned a building on the HK and AM sides into one large room.
- Made it easier for players to get onto roofs.

**S.S. Baroness**

- Removed a floating plank that interfered with wall jumps.
- Moved the exit trigger back slightly, so players must fully enter the room before leaving.

#### v2.1 — Crash hotfix

- Rescripted the vault breakables so the mall can no longer be destroyed all at once, which could cause a crash.
- Removed several more dev textures.
- Updated art in the yellow lane and removed clipping geometry.
