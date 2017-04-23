# Cubase Config Files

Cubase occasionally requires hardware units to be manually programmed. This repository is a collection of those files.

These files are located in the `src` folder. At the moment there are only two.

## Command|8

`src/command8.xml`

The Digidesign Command|8 is designed for Cubase, but includes its own "standalone" mode which provides pared-back commands. However, it is still powerful with its 8 channel strips of touch-sensitive faders, endless rotary encoders, select, mute and solo buttons.

This template must be loaded as a Generic Device, and the Command|8 must be both a MIDI transmitter and receiver  (in order for the faders and encoders to receive automation).

Supports 96 separate channels, which can be accessed via the Generic Device dropdown switcher within Cubase.

Access faders 9 - 16 via the Bank button (located just above the arrow keys).

## Launchpad Mini

`src/launchpadminimap.drm`

Made by Novation, the Launchpad Mini is compact but versatile MIDI controller. As it is intended to work with Ableton Live, its 64 central buttons are not velocity-sensitive, and are thus meant for launching clips - hence the name.

I wanted to use this to select scenes / snapshots in Maschine, but unfortunately its MIDI mappings weren't quite correct. After a day researching MIDI remapping tools, I found that Cubase's Drum Map was perfect for this task.

Only the 8x8 buttons have been remapped to make them perfectly chromatic, starting from C-2.

The top 8 buttons (arrow keys, session, users, mixer) still send the same program changes they always have. The 8 side buttons may have been remapped as a result of changing the primary buttons. They currently send MIDI notes.
