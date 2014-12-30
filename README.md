PushPitch2Mod - Mod wheel for Ableton Push
=============

PushPitch2Mod is a Max for Live device that lets you use Ableton Push's pitch bend touch strip as a mod wheel. The device works on a per-track basis, meaning that you can have the touch strip act as a mod wheel on one track, while retaining Push's default pitch bend functionality on another. Touch strip and LED behavior are changed in Modwheel Mode to simulate a mod wheel.

Installation
-------

Copy PushPitch2Mod.amxd to your Ableton Live user library.

Mac: ~/Music/Ableton/User Library/Presets/MIDI Effects/Max MIDI Effect/ <br />
Windows: \Documents\Ableton\User Library\Presets\MIDI Effects\Max MIDI Effect\

Usage
-------

Connect your Push to Ableton Live, and then drag the PushPitch2Mod device onto the MIDI track you want to use the Push touch strip as a mod wheel on. Your Push must be connected first in order for PushPitch2Mod to discover it.

By default your Push's touch strip will be left in Pitchbend Mode. Enabling the Modwheel Mode either via the toggle switch on PushPitch2Mod, or the encoder mapping on Push ("Ptch2Mod On/Off") with change the touchstrip to Modwheel Mode. In Modwheel Mode your Push's LED strip will act like a mod wheel, and the touchstrip will send MIDI CC #1 (mod wheel) rather than pitch bend.

![Pitchbend mode](https://s3-us-west-2.amazonaws.com/pushpitch2mod/Pitchbend.png) ![Modwheel mode](https://s3-us-west-2.amazonaws.com/pushpitch2mod/Modwheel.png)

Easy!

Known Issues
-------
- The Push touch strip LEDs don't always reset to the correct mode when changing between multiple tracks with PushPitch2Mod devices (though correct the MIDI CCs are still sent).<br />
- Push must be connected before loading the patch or PushPitch2Mod won't see the Push.<br />
- Deleting multiple instances can sometimes lead to crazy LED behavior (try the reset touch strip button and then toggle the mode to remedy this).<br />
- Editing the patch and saving it requires either clicking the bang message in the patcher to restart the selected track detection timer, or deleting and reloading the patch. This seems to be a Max For Live issue, though my remedial Max/MSP patching abilities could just as easily be to blame.<br />
