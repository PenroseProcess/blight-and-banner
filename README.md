Blight and Banner for Enshrouded
=================================

A mod for Enshrouded: new skills and classes (Assassin, Savage, Spellblade), stronger elite enemies, world events and
corrupted loot. It comes with its own build of EMF (the Enshrouded Modding Framework), which it installs with it: you
do not need anything else.

What you need
-------------

- Enshrouded on Steam, on Windows 10 or 11.
- Everyone in a game needs the same build of the mod. The updater (below) takes care of that.

Install (once)
--------------

1. Download BlightAndBanner-<build>.zip from the latest release: https://github.com/PenroseProcess/blight-and-banner/releases/latest
2. Close Enshrouded.
3. Unzip it: right-click the zip, Extract All. Do not run anything from inside the zip.
   Keep the folder: its uninstall.cmd removes the mod later.
4. Double-click "Install Blight and Banner.cmd".
   If Windows says "Windows protected your PC", click More info, then Run anyway (the scripts are not signed).
5. The window finds the game through Steam (or click Browse and pick the folder that holds enshrouded.exe).
   Click Install. It backs up your saves first.
6. When it is done, a "Blight and Banner" shortcut is on your desktop. Click Play now, or start the game with the
   shortcut from now on.

Playing with and without the mod
--------------------------------

- The Blight and Banner shortcut on your desktop starts Enshrouded with the mod. The main menu then says
  "Blight and Banner" and the build in its top right corner, and plays the mod's own menu music. It plays over the
  game's own menu music for now: lower the game's Music slider if the two clash (it sets the mod's music too).
- Steam's own Play button starts Enshrouded without the mod, as if it were not installed.
- A character with a skill above 3/3 that you load without the mod gets its skill tree reset and all its points back.
  Its next load with the mod, in your own world, buys the skills back, as far as your points go.

Updates
-------

They are automatic. Each time you start the game with the shortcut, a small window checks for a new build for a
moment. When there is one, it downloads it, checks the file, backs up your saves, installs it and then starts the
game through Steam. When there is none, the game starts at once.

- Without the internet, or when GitHub does not answer, the window says so and the game starts with the build you have.
  The next start tries again.
- What changed in a build: the release page, https://github.com/PenroseProcess/blight-and-banner/releases

Playing together
----------------

Everyone in the game needs the same build, and everyone starts the game with the shortcut. If you cannot join a
friend, or things behave oddly together, both of you close the game and start it again with the shortcut: each start
installs the newest build. The build you have is on the main menu, in the update window and in
<game folder>\emf\BLIGHT_AND_BANNER_BUILD.txt.

Play together only with friends who run the mod too, or on a server that runs it. A host or server without the mod
lowers your skills to 3/3 or resets your whole skill tree, and saves that into your character. Your next load in your
own world with the mod buys your skills back for you, as far as your points go.

In the game
-----------

- The skill screen shows the new and changed skills with their texts.
- World events roll on one clock for the whole world: a 60% chance every 45 minutes (about one every 75 minutes), for one
  player outdoors, with a 5-minute grace period after loading. The Fell Incursion comes only from that roll, to a player
  inside the Shroud, and its rift no longer fills the air with fog. None comes while you are in a
  base or near a living boss, and you hear an event's music only within 100 m of it.
  Ordinary hostile creatures, including the Fell, have a 1.0% chance to become elites (spaced at least 80 m apart, with a 2-minute cooldown per player).
- Fighting an elite: before a big move, a ring of dots on the ground shows where it will land, and a second ring grows
  until it strikes: step out or dodge. The dots over its emblem are its break bar: every hit fills it, and a parry, a
  backstab, a hit during its warning or a dodged move fill it fast. Full, it is **Opened**: it staggers and takes
  more damage, and a hit at low Health finishes it. Kill it and its followers lose their courage; some run.
- Lure: while sneaking, select it with Next mod skill (Z by default), then hold Use mod skill (G) to aim the teal
  ring. Release to throw the lure there. Next mod skill cancels the aim; the cooldown starts only when you throw.
- The main menu plays Blight and Banner's theme. The game's own music plays normally in a world.
- Settings: press the key under Esc to open the console, then the Mods tab.
- Your skill bar: **K → Skills** opens four personal action slots. Drag a learned active skill onto a slot;
  drag between slots to swap, use X to remove, or Change key to rebind. The default cries are **F Seismic**,
  **G Enduring**, **R Infernal**, **T Ancestral**. Each slot shows its key and cooldown. Your layout follows you
  between worlds and friends' games; editing it never resets a cooldown. Assigned skill keys take priority during
  play. Menus, chat and building keep their usual controls. Banner, HUD and Controls are tabs in the same window.
- Combat hints: **K → HUD → Combat hints** turns floating combat messages on or off. Choose which groups to see:
  damage and numbered effects, healing and recovery, resource costs, or status messages. **Group repeated messages**
  combines the same effect on one target within 0.6 seconds and adds its numbers. These choices save immediately
  on your PC and work in friends' games too. The first-time tutorial cards have their own switch above this section.
- Your banner: press K (the Mod menu key) in a world to pick your Notoriety banner's colour and emblem in a window
  (also in a friend's game); K, Esc or Done closes it. The other players see your choice within a few seconds. "From
  my name" gives you the colours your name picks. "Show my banner over my head" hides or shows your own banner
  above you (your rank stays on your HUD). Typing co.banner in the console opens the same window.

Your saves
----------

- Before each install and update your saves are copied to %LOCALAPPDATA%\EMF\save-backups (the first one is called
  "Before EMF" and is kept; of the automatic ones the newest ten are kept). The game also makes one when it starts
  with the mod and a save changed since the last one (at most once an hour).
- To restore a backup by hand: close the game, open the backup's folder, and copy each file back to the same name:
  steam\<id>\<file> to <Steam>\userdata\<id>\1203620\remote\<file>, and local\default\<file> to
  %USERPROFILE%\Saved Games\keen games\Enshrouded\default\<file>. Copy the files you replace somewhere safe first.
- Uninstalling never deletes the backups.

What it installs, and what it contacts
--------------------------------------

- In the game folder: dinput8.dll and the emf folder.
- The updater: %LOCALAPPDATA%\BlightAndBanner (it lives outside the game folder, so a game update or a reinstall of
  the mod never breaks the shortcut), and the shortcut on your desktop.
- At each start with the shortcut the updater asks GitHub for the latest release (api.github.com, and GitHub's
  download server when there is a new build). It sends nothing about you or your PC. The mod itself contacts nothing.

Problems
--------

- The shortcut does nothing, or it is gone: run "Install Blight and Banner.cmd" again; it makes the shortcut again.
- Steam asks whether to allow starting Enshrouded with "-blightandbanner": that is the shortcut. Allow it.
- The main menu does not say Blight and Banner: the game was started with Steam's Play, so the mod is off. Close the
  game and start it with the shortcut.
- "Could not update": the window says why. The game starts with the build you have; the next start tries again.
  GitHub allows about 60 checks an hour from one address.
- The game crashes or the mod does not show: send the logs below. To play without the mod meanwhile, start the game
  with Steam's Play.
- Your antivirus removed dinput8.dll: mod loaders are sometimes flagged by mistake. Allow it, or install again.
- What to send when asking for help: <game folder>\emf\emf_core.log and %LOCALAPPDATA%\BlightAndBanner\updater.log.

Uninstall
---------

1. Delete the Blight and Banner shortcut from your desktop (otherwise its next start installs the mod again).
2. Close the game, then double-click uninstall.cmd in the unzipped folder (or download the zip again for it).
   Your saves and settings stay. Without the mod the game resets the skill tree of a character with a skill above 3/3
   and gives all its points back. Installing the mod again buys the skills back, as far as your points go.
3. Delete %LOCALAPPDATA%\BlightAndBanner (the updater and its log).

Without automatic updates
-------------------------

install.cmd in the unzipped folder installs that build without the window, the updater and the shortcut. Then you
install each new build yourself, the same way. To start the game with the mod, put -blightandbanner into Steam's
launch options for Enshrouded (Library, right-click Enshrouded, Properties, General); without it the game starts
without the mod.
