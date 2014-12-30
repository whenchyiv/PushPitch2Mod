PushPitch2Mod - Modwheel for Ableton Push
=============

PushPitch2Mod is a Max for Live device that lets you use Ableton Push's pitchbend touch strip as a modwheel. The device works on a per-track basis, meaning that you can have the touch strip act as a modwheel on one track, while retaining Push's default pitch bend functionality on another. Touch strip and LED behavior is changed in modwheel mode to simulate a modwheel.

Installation
-------

Copy PushPitch2Mod.amxd to your Ableton Live user library.

Mac: ~/Music/Ableton/User Library/Presets/MIDI Effects/Max MIDI Effect/ <br />
Windows: \Documents\Ableton\User Library\Presets\MIDI Effects\Max MIDI Effect\

Usage
-------

Connect your Push to Ableton Live, and then drag the PushPitch2Mod device onto the MIDI track you want to use the Push touch strip as a modwheel on. Your Push must be connected first in order for PushPitch2Mod to discover it.

By default your Push will continue to send pitchbend to the track. Enabling the Modwheel mode either via the toggle switch on PushPitch2Mod, or the encoder mapping on Push ("Ptch2Mod On/Off") with change the touchstrip LCD to a modwheel, and send MIDI CC #1 (modwheel) rather than pitchbend.

![Modwheel mode](https://s3-us-west-2.amazonaws.com/pushpitch2mod/Modwheel.png)  ![Pitchbend mode](https://s3-us-west-2.amazonaws.com/pushpitch2mod/Pitchbend.png)

Simple!

Known Issues
-------
- Touchstrip sometimes doesn't reset to correct LED mode when changing tracks (though correct CC is still sent).<br />
- Push must be connected before loading the patch or PushPitch2Mod won't see the Push.<br />
- Deleting multiple instances can sometimes lead to crazy LED behavior (try the reset touchstrip button and then toggle the mode to remedy this).<br />
- Editing the patch and saving it requires either clicking the bang message in the patcher to restart the selected track detection timer, or deleting and reloading the patch. This seems to be a Max For Live issue, but my remidial Max/MSP patching could just as easily be to blame.<br />
