## Page 1

[*REFERENCE Basic Audio Recording*](/Sound/Basic%20Audio%20Recording/)

### Frequency and Amplitude
- 20-150Hz - low frequencies (boomy, dark, bassy)
- 150-800Hz - low mid frequencies (warm, muddy)
- 500-800Hz (barky)
- 800-4kHz - mid frequencies (harsh, nasally)
- 4-8kHz - hi mid frequencies (sibilant, somewhat bright, rough)
- 8-20kHz - hi frequencies (bright, airy)
- *These ranges are not absolute*

- Complex waveform: the fundamental frequency plus itself to infinity (its harmonics).
- All frequencies involved make up the tone or timber
- The fundamental frequency determines pitch.
- The fundament is also called the first harmonic ex. 440Hz (fundamental, 1st harmonic) -> 880Hz (2nd harmonic) -> etc.
- The fundamental is the strongest and the subsequent harmonics get softer.

- A decibel is the way we express a ratio of SPL Intensity.
- 0dBSPL threshold of hearing.
- 10 log⁡(P1/P2)
- 10dBSPL is 10 times greater than 0dBSPL, 20dBSPL is 100 times greater than 0dBSPL, etc.
- Normal conversation is approximately 50-60dBSPL.
- Small parties can be around 70-75dBSPL.
- Typical concert can be 105-120dBSPL.


## Page 2

- 85 dBSPL is the point that human hearing responds to frequencies the flattest.
- Human hearing tends to be most sensitive 1-5kHz (where most of the pronunciation, diction, and annunciation comes into play).

  

### Sound System Signal Flow

- Source -> Pre-amp -> Processing -> Power Amp -> Speakers -> Ears
	- Source: Mics, Sound Waves
	- Pre-Amp+Processing: Console
	- Power Amp: Console Output
	- Speakers: Power Amp Output
	- Ears: Sound Waves from speakers

- 3 standard audio reference levels
	- Mic: -30 - -60dBu
	- Line: +4dBu
	- Speaker: Watts

  

### Electricity

- Components:
	- Voltage (Volts) - the potential for how much electricity can flow
	- Current (Amps) - the electrons flowing through the cable, positive and negative flows.
	- Resistance (z) / Impedance (ohms) - what resists the electron flow

- DC - Direct Current, one way positive flow.
- AC - Alternating Current, having both positive and negative flows.
- Ohm’s Law: Voltage = Current x Impedence | Current = Voltage / Impedence | Impedence = Voltage / Current
- Watts - the “work”, how much power, capable of being produced.

### Mics

- Dynamic
	- Passive device (doesn’t need any excess electronics to work)
	- Most will be one polar pattern
	- Colder output compared to condenser mics
	- Higher Impedence values
	- Cost less
	- Less fragile
	- Slimmer frequency response

- Condenser
	- +48VDC
	- Various polar patterns (optional)
	- Hotter output compared to dynamic mics
	- More expensive
	- More fragile
	- Wider frequency response

- All professional mics will have an Impedence value of less than 600ohms.
- Matching Impedence values is the easiest way to transfer audio from one piece of gear to another. Mic output to Mic-Pre input < 600ohms.

- Wireless Mics
	- Head of the mic is called the transmitter that takes in SPL and turns it into an infrared signal, the signal goes to the corresponding receiver and the receiver turns the infrared signal to an audio signal.
	- Systems with 2 antennas are called diversity systems.

### Feedback

- Amplified sound renters a mic at the same or greater level than the direct sound.
- There’re a few frequencies that reflect more than others.


## Page 3

- Head Room = Peak Levels Needed - the Nominal Operating Level
- DI - Direct Injection Box
	- Changes an Unbalanced High Impedance Input signal into a Balanced low Impedence Output signal.
- Instrument pick-up’s tend to be unbalance connections with high Impedence.
- Transformer: A piece of equipment that has a series of windings in a coil around an iron based core and a series of output windings. The input windings can be different from the output windings depending on what the user is looking to change about the input.
- In a Balanced Cable; pin 1 is always ground, pin 2 and 3 can be the Hot (the line carrying the positive signal referencing the ground) pin depending on how the equipment was assembled.
- In an Unbalanced Cable; pin 1 is the ground and pin 2 or 3 carries the audio.


## Page 4

### Console

- Inputs
	- Inputs: mic input, line input, AES, MADI, Dante

- Routing: assigning all inputs to outputs

- Output/Master
	- 1 bus -> mono master
	- 2 mix bus/stereo bus/main bus/master bus -> master fader
	- Other outs: subgroup/group, Aux Send (buses to create additional mixes (can be pre or post fader))
	- Outputs from pro consoles are Balanced, Line Level, and High Impedence.

- Dynamics
	- Outboard gear (aux send and input channel return)<line level, balanced>
	- Insert (a send and return in one circuit)<line level, balanced>

- VCA - Voltage Control Amplifier
	- No audio is flowing through the VCA only electronic control. Only level control and mutes. Serves as a fader to make mixing condensed and easier.

- TRS - Tip Ring Sleeve
	- Tip is positive (audio), Ring is negative (audio phase reversed), Sleeve is ground

- TS - Tip Sleeve
	- Tip is audio, Sleeve is ground

- IEM - In Ear Monitor

- Audio ISO Splitter
	- Has inputs and grouped outputs. I.e. 2 groups of outputs = 2 way iso splitter.
	- The number of individual outputs is implied by how many inputs. I.e. 56 in/56 out (per group).
	- ISO transformers:
		- Blocks DC Voltage (only the direct connection will be able to supply phantom power)
		- Isolate reactance between consoles.
		- Provide pin 1 (ground) lifts on every channel.


## Page 5

- PAD is also known as an Attenuator.

  
### Drivers

- The raw speaker is called a driver in pro audio terms.
- Speakers have a center dust cover (as it sounds), paper cone, suspension (to help from blowing and over extending the paper cone, and frame (what allows the driver to be mounted), leads (where the audio current enters, is an unbalanced connection (like the output of power amps)).
- Drivers are Output transducers (voltage and current to SPL).
- The Permanent magnet in a drive assembly surrounds a coil of wire called the voice coil. Once current is applied to the voice coil a secondary magnetic field is created causing the the permanent magnet to attract and detract the voice coil resulting in movement of the voice coil (or more specifically the small metal cylinder residing in the voice coil, and that cylinder push the diaphragm for the driver cone). Multiple drivers make up a speaker.

- Drivers come in different types:
	- Woofer
	- Low frequency driver
	- Mid frequency driver
	- High frequency driver
- Different sized drivers from every manufacturer have different frequency responses that they work best at.
- Different Drivers have different levels of power handling (how many watts the internal components can handle from the power amp).

- Measured in 3 different ways:
	1. Program - how long it handles a constant input of watts over a period of time before is degrades.
	2. Peak - how much wattage the internals could take in an instant without breaking down.
	3. Continuous - somewhere in between program and peak.
- Drivers have differing levels of Sensitivity (how efficient the driver is at converting watts to dBSPL) (should be tested on-axis)

- Drivers have a spec called Dispersion Pattern; how many dB in what frequency range are gained or lost as one gets off axis.

- Different drivers have different Impedence values. Nominal Impedence (average Impedence).

  

### Audio Crossover - divides frequency bandwidths which then goes to separate drivers.

- Passive Crossover: internal component of the speaker cabinet. Designed by the manufacturer. Fixed frequency ranges. High current speaker level. These tend to be full range speakers.
- Active Crossover: External piece of gear. Line level in/outputs.

### Power Amp

- Power Handling - Watts (this time how much power can it deliver without breaking down)
	1. Peak
	2. Program
	3. Continuous

- Bandwidth - what operating frequencies does it work best in

- When pairing amps and speakers you want an amp that can sent double the wattage of the speakers.
- Current can only flow one direction; linking together multiple speakers to carry the same information is called a series circuit; but the Impedence values are added together, putting a greater load on the power amp.
- Parallel circuit: the positive terminal of the amp is wired to the positive terminal of the first speaker and to the positive terminal of the second speaker, the negative terminal of the amp is wired to the negative terminal of the first speaker and to the negative terminal of the second speaker.
- Damping Factor: the spec that helps control the oscillation of a driver to negate unnecessary oscillating of the driver creating false sound waves. Affects low frequencies. High factors are better.
- Slew Rate: a rate of time; time from input to output. How quickly the amp amplifies the signal. Affects high frequencies most. Lower rates are better.
- “One Legged” - only 2 of 3 pins are working in a cable.


## Page 6

### Sound Distribution

- Speakers have a dispersion pattern that they radiate sound in. These specs are given on a 360 degree graph. A typical patten is 90 degree width by 30 degree height.
- A common speaker cabinet design is trapezoidal so as to widen the dispersion pattern and couple together to disperse sound as one unit when pushed flush together.
- Throw - the distance a speaker can send sound.

- Line arrays - speaker cabinets that are stacked sideways on top of each other so that each corresponding frequency driver is vertically in line with the others of the corresponding frequency driver. Most line arrays are hung for events and are hung in a “J array”. To evenly distribute dBSPL in a line array, “shading” is used at the power amp stage to add or reduce level down the line array.

- Critical Distance Point - the point in a venue where reflections are equal to or greater than the direct sound.

- Front loaded drivers - the drivers are up against the grill (the front) of the cabinet.
- Horn loaded driver - a “horn” is is an acoustical impedence device. It disperses the air mass at the flare of the horn to reduce the air molecule Impedence. The driver is mounted to the horn which is mounted to the grill of the cabinet.
- Zones - zones of coverages that our speakers are filling. The different zones tend to be placed on different busses. The zone fills are likely to be different mixes based on perceived acoustical sound.

- Matrix - a way of mixing mix-busses.