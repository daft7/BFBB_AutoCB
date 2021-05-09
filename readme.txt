AutoCB v1.1R2 by fuse and daft7

Revision 2

Added camera angle (C) to debug screen
-convention is aligned with facing angle on level load/directly behind character, increases as you move clockwise around the character
Added Hand on Demand with RT + black

Revision 1

AutoCBs now behave as intended, issue was that the value for bowl dampening was nonzero causing slowdowns
Old AutoCB (replicating LT+B) is back and is activated by RT+white
Positive side effect of this is saving/warping can now be disabled by holding RT should you want to use debug fly via black button

Features and changes from 1.0:

**Many controls have been changed to accommodate new features and future plans
AutoCB is now RT + Up on Dpad, Up still increases speed by 1 as before but must be in CB state and not holding RT (i.e., entering CB does not give you +1 speed)
Hans enable/disable now RT + Down on Dpad, disabling still gives shiny as indicator
Save coords/Warping now white/black button, warping should now clip through collision
Moon jump: enable/disable on RT + Y, hold A to rise when enabled
Debug fly: enable/disable on RT + B
Kill combo: RT + A
Character swap: now RT + back

"Debug" screen: displays XYZ to hundredths; Facing angle, Thumbstick angle, and Y momentum to tenths,
	status of Moon Jump and Debug Fly, and a frame counter
Show/hide by RT + right thumbstick click
Reset frame counter by RT + left thumbstick click (warping also resets the frame counter)

Can now do character swap for Robo-Sandy and Robo-Pat
No longer awarded a spatula for every five minutes of play :(
Version info text now works as Tetrax's, slightly transparent on gameplay and solid on pause (speedometer remains solid)


Installation:
Go to https://www.marcrobledo.com/RomPatcher.js/ or use a tool that supports IPS patching (Lunar IPS, IPSEXE, etc.)
Input your default.xbe and the default_autocbv1_1.ips file, output your modified xbe
default.xbe likely has to be NTSC-U, outputted xbe is supported on both original hardware and CXBX


Known issues:
(fixed)Speedometer does not always match bowl state speed, unknown why, CBs without mod assistance seem to be accurate while those with the assist may not be.
-the presence of the bowling pin on the ground seems to indicate that it is inaccurate
Debug screen had issues in testing with lines getting filled with garbage characters, should be fixed
-In cases where issues arose, reloading the level seemed to correct this.
Getting pulled by Hans with debug fly mode on disables debug fly but it still displays as ON. Toggling again fixes this.
Could cause crashes but this may have just been emulation
Debug screen text could get messed up with addition of camera angle
Hand on Demand may not always work, try reloading the level if it does not


Notes:
HUGE thanks to tenfivehunnit for digging through memory
Warp clipping is accomplished by enabling debug fly while holding the black button; exploration is possible this way but likely easier with enable/disable.
Utilization of RT and moving warp off Dpad was done to prevent accidental presses and allow for the use of the Dpad to line up tricks
Debug fly controls: powers disabled, X/Y to decrease/increase height. Holding either trigger increases speed.
-This does cause a bit of a control conflict. It is recommended to increase speed with LT or just be aware that moon jump may toggle if rising while holding RT.
Angle conventions:
-Facing is 0 when moving along the positive Z axis, increases as you turn clockwise
-Thumbstick is 0 straight up, again increasing clockwise (resting at 90 due to conversion)
Compatible with Tetrax's Practice Mod
xbe was renamed in a hex editor, not sure if that will display