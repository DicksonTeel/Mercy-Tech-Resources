# Advanced Signal Flow Principles

## New Concepts

### Insert
- An access point into the signal flow of a channel.
- Allows for connections of plugins or external outboard gear.
- EQ and Dynamics
- Has 2 components:
	- Send - gets signal out of the flow.
	- Return - returns signal to flow.
	- The signal returns at the same point from which it left.
	- In the analog world these will be patch cables. In a DAW, these are handled in the background.
- Characteristics
	- Process the signal in its entirety - you hear 100% of the processed signal.
	- Channel by channel basis - every channel has 1 or more inserts and it is exclusive to that channel.
	- EQ & Dynamics (mostly, 99%).
	- “Do” I’m doing something to the signal; changes the original signal.
	- Inserts are a serial process (one after the other).
	- No send or return level controls are apart of the Insert itself (certain outboard gear and plugins may have these).
- Can Be Found On
	- Individual channels
		- Input or monitor
	- Stereo Bus
	- Subgroup Masters
### Auxiliary Send
- Send a portion of the signal flow onto a bus.
- Controls: Send level / mute / pan / Pre/Post switch.
- Console wide - the aux bus is available to all channels.
- Signal will not return to its original location. Instead it will come back into the signal flow separately.

### Auxiliary Return
- The aux send feeds to the desired outboard gear.
- The output from that gear will need to return to the stereo mix bus in order to be heard. May be a channel or dedicated aux return.

### Aux Send & Return
- Typically used for “time based effects”.
- “Add” I’m adding something to the original signal.
- Parallel in nature. Original signal (dry) and Processed signal (wet) get mixed together.

### Groups
- Control
	- VCA (Voltage Control Amplifier) “Style” groups.
	- Used for pure volume.
	- DAWs use Mix/Edit groups for the same style of control.
- Consoles
	- Subgroup
		- Combine or “Submix” tracks using a bus; either a Multi-Track bus or alternate Stereo Bus.
		- Will combine with the rest of the mix at the Stereo Bus.

### Soloing
- Gives us the ability to listen to channels/groups/buses by themselves
- Destructive - solos one channel by cutting the rest, thereby leaving only one channel to listen to. Does not use a separate bus. SIP - Solo In Place. SIF - Solo In Front (Dims the other tracks instead of cutting them). Solo Safe/Isolate - Tells soloing system that user selected channels are not to be effected by entering solo mode.
- Non-Destructive - PFL - Pre Fader Listen, can hear channels even if the fader is down. Level soloed is not always the same level being monitored. AFL - After Fader Listen, you hear the level of the channel as it is in mixing.

### Patch bay
- A series of female jacks that connect to all of the gear in a studio; this creates a centralized place where all gear I/O can be accessed. Access is gained by plugging a male patch cable into any of the female jacks.
- Outputs on top of rows, inputs on bottom of rows.
- Normals
	- Full Normal
		- Patch into either top or bottom row breaks the normal.
		- Mic lines to mic inputs.
	- Half Normal
		- Patch into bottom row breaks the normal.
		- Patch into bottom row does not break the normal.
		- Console to multi-track, multi-track to console.
	- No Normal
		- No connection between the top or bottom rows.
		- Outboard gear.