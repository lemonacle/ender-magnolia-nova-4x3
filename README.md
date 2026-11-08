# ENDER MAGNOLIA: Steam version — Retroid Pocket Nova 4:3 settings

This settings file enables the game's internal 4:3 camera option when playing the Steam version through DroidDeck on a Retroid Pocket Nova. Tested on Steam build 17867309 (game version 1.1.1).

This is an experimental settings workaround. The camera accepts 4:3, but the interface and framing are not fully polished for this aspect ratio. This file does not patch the game executable or set the launcher's output resolution.

## Included file

- `SettingsSlot.sav`: modified Nova settings file with `EConstraintCameraAspectRatio::CameraAR_4_3` added. It is based on one device's exported settings, so replacing your file also adopts that file's other preferences and controller bindings. It is not a gameplay-progress save.

## Install on the Nova

1. Close ENDER MAGNOLIA completely.
2. Transfer the included `SettingsSlot.sav` to an accessible folder on the Nova, such as Downloads or the SD card.
3. Open Android's Files app. In the side menu, select **DroidDeck**, then open **files → steam-libraries**.
4. Open your library's long folder name, then follow the path below. `<LIBRARY_ID>` is a placeholder: use the existing long folder name on your device. Do not create or rename this folder. If there are several library folders, find the one containing `steamapps/compatdata/2725260`.

```text
DroidDeck/files/steam-libraries/<LIBRARY_ID>/steamapps/compatdata/2725260/pfx/drive_c/users/steamuser/AppData/Local/EnderMagnolia/Saved/SaveGames/
```

5. Back up the existing `SettingsSlot.sav` to a separate folder before replacing it. Keep this backup so you can restore your original preferences.
6. Copy the included `SettingsSlot.sav` into that SaveGames folder and approve replacement. Leave any other save files untouched.
7. Launch the game and check gameplay, HUD, map, and menus. Use a 4:3 output resolution in your launcher if needed; this settings file only controls the camera aspect ratio.

The library identifier is installation-specific. The game files can be on the SD card while this settings folder is in DroidDeck's private internal storage. Browse through the DroidDeck entry in Files rather than looking only in the SD card's game installation folder.

## Keep the hidden setting

Avoid changing the in-game aspect-ratio selector after installation: selecting one of its exposed options may replace the hidden 4:3 value. The menu does not expose a supported 4:3 choice.

## Restore

Close the game, then copy your own backed-up `SettingsSlot.sav` back into the same SaveGames folder, replacing the modified file.

## Scope and limitations

- For the Steam version running through DroidDeck; other launchers have different save locations.
- Tested on a Retroid Pocket Nova, with remaining layout/framing issues observed during testing.
- This is a shared settings preset, not a complete 4:3 mod or a patcher that preserves each recipient's individual preferences.
- Do not replace unrelated gameplay saves. The Steam app ID for this game is `2725260`.

