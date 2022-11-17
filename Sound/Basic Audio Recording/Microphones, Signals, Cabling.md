# Microphones, Signals, Cabling
- Microphones are precision devices.
- Often abbreviated as Mic or Mics.
- A mic is a transducer (changes one form of energy into another).
	- Change acoustical into electrical energy

**There are several “types” of mics; defined by how they transduce**
**We will study 3 types:**
- Dynamic
- Ribbon
- Condenser

## Dynamic Mics

- Uses magnetic induction
	- Pass a magnetic field through a conductor, it generates electricity (mic)
	- Pass electricity through a conductor, it generates a magnetic field (speaker)
- Sound causes the internal diaphragm to move
	- The diaphragm moves a coil (a conductor)
	- The coil is mounted in a magnet
	- Movement of conductor in the magnetic field creates electricity
- Very rugged, both physically and sonically
- Handles very high SPL

## Ribbon Mics

- Works on magnetic conduction
	- Lightweight ribbon mounted between two magnets
- Very fragile (drops and wind can damage)
- Give a smooth frequency response

## Condenser Mics
*aka “Capacitor mic” (no one uses this terminology anymore)*

- Capacitor: stored an electrical charge
	- Charge is stored between the diaphragm and a backplate
	- Sound moves the diaphragm, changes the output
- Very sensitive
- Excellent transient response
	- Transient response (how it handles rapid changes in amplitude)
	- Handles high SPL (may have an internal pad to avoid distortion in electronics)
- Small Diaphram Condenser (SDC)
- Large Diaphram Condenser (LDC)

**Dynamics are usually for up close/Condensers are usually for further away**

---

## Microphone Properties
### Phantom Power (±48V)

- Voltage sent down a mic cable, in opposite direction of audio. Provides change to plates and amp inside a mic.
- Does not interfere with the audio signal.
- Has no effect on dynamic mics, but do not put phantom power on ribbon mics as it may damage them (unless it’s an active ribbon which will require phantom power).

### Polar Pattern

- Sensitivity at various angles with respect to the front of the mic
- Sensitivity: output level compared to input
	- Higher sensitivity = higher output
- Polar pattern aka Polar response or Directional response.
	- 2 Categories:
		- Omnidirectional: Picks up equally in all directions
		- Directional: Pick up sound better from some directions than from others
	- Directional patterns include:
		- Unidirectional
			- Cardioid: Picks up sound in front; rejects rear
				- Named for inverted heart (“cardio”) pick-up shape
			- Super/Hypercardioid: Better side rejection than cardioid
				- Best rejection at 120 & 140 degrees
				- Some rear pickup
	- Bi-Directional (figure 8)
		- Pick up sound equally well at front and rear
- Frequency response and polar response diagrams only give a general idea of a mic characteristics, it is still up the the engineer to choose what is best for each situation.

### Self-noise

- All electronic devices produce noise, some more than others. Mics don’t produce much self-noise, but it is still there (ribbons and dynamics have the least).

### Proximity effect

- An increase in bass response as a directional mic is moved within 1ft of a sound source.
- Omni’s don’t have this.
- The proximity effect is a byproduct of directionality.
- Your options:
	- Use it to your advantage
	- Move the mic
	- Highpass Filter
	- Use a bass roll-off switch on your mic (sound of an Omni, pattern of a cardioid)
	- Change polar patterns

---

## Microphone Techniques
### Close mic’ing

- Created tight, present sound
- Effectively excludes the acoustic environment 
- Reduces “leakage”
- 3:1 rule: To minimize phase problems, for every unit of distance between a mic and its source, a nearby mic should be at least 3 times that distance

### Ambient/Room mics

- 50/50 or greater relationship between reflected and direct sound
- Provides natural reverberations (the sound of the room)
- Often use stereo mic technique
- Can be used alone or with close mic’ing

### Stereo Mic’ing

- Spaced Pair (A-B Stereo)
	- Most basic stereo technique
	- Usually same make and model mic
	- Stereo image derived from time & amplitude cues
	- Drawback: potential for phase discrepancies

- X/Y
	- 2 directional mics, same make and model (commonly cardioid)
	- Placed as close together as possible without touching
	- Angled from 90-135 degrees
	- Midpoint pointed towards the source
	- Panned equally left and right
	- Image is not as wide but there are no phase problems

- Blumlein
	- X/Y with 2 bidirectional mics
	- Excellent ambient results

- M/S (Mid/Side)
	- Cardioid mic (mid) facing source
	- Bidirectional mic (side) positioned with null facing source
	- Excellent mono capabilities (minimal reverb)

## Mic Level vs Line Level vs Instrument Level

- Mic level - a range of voltages that are lower in level than line level (approx -60 to -40dBu)
- Line level. Typical running level through most equipment aka nominal operating level (+4dBu)
- Instrument level - varies widely, sometimes down with mic level and sometimes approaching line level. Older passive pickups vs modern active pickups.

- Impedance
	- Impedance is the measure of the total opposition to current flow in an alternating current circuit. It is made up of the sum of 2 components, resistance and reactance.
	- Measured in Ohms
	- 2 worlds: high impedance and low impedance
	- High: subject to noise and high frequency loss in cables running longer than 25ft. Most instruments have high impedance outputs.
	- Low: less subject to noise or frequency loss over longer running cables.

- Balanced vs Unbalanced Signals
	- Unbalanced cables are subject to noise as they are only single coil cables
	- Balanced cables add a second coil that reverses the signal phase and the device input flips one around resulting in a clean signal.

- Direct Injection Boxes
	- Has a high impedance, unbalanced instrument input
	- Has a low impedance, balanced, mic level output
	- Have better isolation that gives a cleaner, more present sound than most mic techniques allow
	- Come in 2 flavors: active or passive

- XLR Connectors
	- Usually low impedance
	- Balanced connections
	- Mic or line level
	- Are a directional cable

- 1/4” TS or TRS Connectors: “tip/sleeve” Or “Tip/ring/sleeve”
	- Instrument cables
		- High impedance (TS)
	- TS cables are unbalanced
	- TRS cables are balanced
	- 1 balanced Low impedance (TRS) OR Stereo, High impedance (TRS)

---
## Other Resources

- How It’s Made: Microphones