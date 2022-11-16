# Principles of Signal Flow

Signal Flow: the framework of ALL audio-engineering
There are many facets to signal flow. Today will only discuss what is needed to do basics and overdubbing. Mixing will be covered at a later date.

## What is a Buss(bus)?
- At certain points in the signal flow, signals must be combined or “mixed” together. Signals are combined by feeding the signals to a “Bus”. A bus can accept many signals at its input and combine together into one output.
- The are 3 types of Buses
	1. Stereo Bus - what makes your 2-track mix.
	2. Auxiliary Send - used to make “headphone” mixes and to add certain types of “effects”.
	3. Multitrack Bus - a bus used to combine mic’s/Direct Injection Boxes during recording or to create sub-mixes/groups.

- 5 initial Signal Flow Concepts
	1. Input path/section: microphone/DI-Box to multitrack recorder, 1 for each mic.
	2. Monitor path/section: from multitrack recorder to stereo bus, 1 for each track.(engineer’s mix)
	3. Cue or Headphone path/section: using aux sends to create a discrete headphone mix, 1 for each track.(artist mix)
	4. Masters section: a collection of bus masters. (ST,aux,MT)
	5. Monitor (speaker) Controller: either a part of the console, interface, or a stand alone device that is responsible for what comes out of speakers and more.
- Input Section
	- The mic pre, short for microphone preamp, provides the following for mic/DI signals:
		- Gain - boosting the signal from the mic to the line level
		- Phantom Power - +48v for condenser mics or certain DI-Boxes
		- Pad - attenuation for high output mic signals
		- Phase Reverse - 180 degree phase reversal of the signal
		- *features may vary*
	- Input sections can sometimes accept sources other than microphones such as line level or instrument level signals.

	- Opt Proc AKA Optional Processing AKA EQ/Dynamics.

	- Input fader - not present in all situations (hardware dependent)
		- The input fader gives level control over signals bound for the multitrack. Typically, the input fader is set at “unity gain” or 0dB. This way, the fader neither adds nor subtracts from the signal.
		- The input fader is used to provide balance control of signals being combined together using a multitrack bus.

	- Routing (on consoles)
		- Routing determines how signals make their way to the multitrack recorder and which track(s) they are sent to. There are 2 ways this can be done:
		- Direct Out -  one input signal goes to one track of the multitrack, no signals are combined.
		- Pan and Bus Assignment - multiple input signals are combined together and recorded onto a single track. A multitrack bus is used to do this.

	- Routing (with DAW’s)
		- With DAW’s it is often as simple as selecting the input via a menu that your mic is plugged into.

- Monitor Section
	- The monitor section receives signals from the multitrack and routs them to the stereo bus. This can be though of as the “engineer’s mix” and a possible basis of a “final mix”
	- It is made up of:
		- Optional Processing (auditioned but not recorded)
		- Monitor fader - level control
		- Pan - left/right placement
		- Routing to stereo bus

- Masters Section
	- Provides level control over all buses present in the signal flow.
	- These include:
		- Master fader master
		- Multitrack bus master
		- Aux/Cue/FX (send) master
	- Every bus must have a master level control, but every bus has a master.

- Monitor Controller
	- The monitor controller section provides control over signals going to the control room monitors.
	- These controls are:
		- Monitor source: stereo bus, 2-track return, CD, iPod, etc.
		- Monitor mode: mono, stereo, surround
		- Speaker select: main, alt, mini, etc.

	- Communications:
		- Talkback - engineer to artist communications
		- Listen mic - studio to control room communications (either a part of the console or a dedicated setup)
		- Auto TB, Auto Listen - tied to Transport

- Cue Section:
	- The cue path takes signals coming from the multitrack recorder and sends them to the headphones. The cue path is apart of yet separate from the monitor path.
	- The cue path is made up of:
		- Cue send with pan
		- Cue master
		- Talkback is injected at monitor controller

- The Mixing Console
	- A mixing console is a device that contains all of the components of signal flow in one piece of equipment, there are 2 main types of consoles defined by how they handle “monitoring” - Split and Inline