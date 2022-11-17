# Physics of Sound

- Psychoacoustics - phenomenon that effects how the brain perceived sound.
- Sound waves are variations in atmospheric pressure.
- Wave propagation - sound moves through a medium (air) in a 3-d, spherical pattern.

  

## Compressions & Rarefactions:

- Small shifts in atmospheric pressure.
- Compression: air molecules move closer together.
- Rarefaction: air molecules moving farther apart.

## Waveform

- Graphical representation of sound-pressure over time.
- Also applies to voltage and digital audio.
- Waveform Characteristics
	1. Frequency - each wave completion is called a cycle.
		- Hertz (Hz) [the unit of measure] - the number of cycles that occur in 1 second.
		- Related to Pitch and Tone
		- Frequency rage of human hearing: 20Hz - 20,000Hz AKA 20Hz - 20kHz
			- 1000 Hz = 1kHz

	2. Amplitude - the maximum extent of a vibration or oscillation, measured from the position of equilibrium.
		- Essentially is the volume.
		- Represented by the height above or below the center line.
		- Decibel (dB) [the unit of measure]
			- Comparative unit of measure = always comparing something to something else
			- Sound pressure level (dBSPL)(threshold of hearing, discomfort, pain)
			- Signal Level (voltage - dBu, dBv, dBV, dBmV, etc.)
				- dBu - pro audio
				- dBV - consumer audio
				- dBFS - digital audio
			- There will always be a reference level (often implied)
			- An increase of…
				- .5 to 1dB is barely noticeable to most ears
				- 10dB sounds twice as loud (psychoacoustic)
				- 6dB is truly twice the pressure
			- Why we use dB:
				- Ear operates over a wide range of levels (approx. 10^13:1)(not a user-friendly number). The need of a method to reduce these larger values to smaller, more manageable numbers.

	3. Velocity - how fast sound travels (1125-1130 ft/sec (increases with temperature))<the triangle of 1’s = 1kHz:1ms:1ft>
		- Frequency impacts velocity.

	4. Phase - Identifies the various points in a cycle
		- Measured in degrees.
		- Frequency dependent.
		- With only one signal, phase doesn’t have any implications. With 2 or more “phase related” signals, relative phase between them comes into play.
		- With 2 related signals:
			- Relative amplitudes are often different at any one point in time.
			- Relative amplitudes combine; reinforcing or cancelling each other.
		- When 2 waveforms have the same frequency, shape and peak amplitude (this is called being in-phase). The resulting wave has the same frequency, shape and phase the amplitude will be doubled. If the waveforms are 180 degrees out of phase, the cancel completely.
		- If the second wave is partially out of phase…
			- Constructively interfere where amplitudes are that same.
			- Destructively interfere where amplitudes are different.
		- Phase Shift
			- Arrival time differences.
			- May be in-phase at some frequencies and out-of-phase at others.
			- Boosts and cancellations alter frequency response.
		- Frequency Response - a graphical output over a range of frequencies; shows the effect of a device on tone.
			- Measurement:
				- Input constant amplitude signal swept over entire frequency range.
				- Measure device output at each frequency.
				- Flat (linear) frequency response: output amplitude is same at all frequencies.
				- Colored (non-linear) response: output amplitude differs at certain frequencies.

	5. Simple Waves
		- Continuous and repetitive.
		- Symmetrical around the 0 line.
		- Not naturally occurring.
		- Example:
			- Sine wave
				- Single frequency
				- Specific pitch
				- Pure sound
			- Square wave
			- Triangle wave
			- Sawtooth wave

	6. Complex Waves
		- Don’t necessarily repeat
		- Rarely symmetrical
		- Contains multiple frequencies
			- Fundamental
			- Harmonics
			- Partials and overtones
		- All naturally occurring sounds are complex.

---
**Timbre (“tamber”) - the combination of qualities of a sound that distinguishes it from other sounds of the same pitch and volume.**
	Contributing factors:
	Harmonic content & other overtones
	Relative amplitude of these frequencies
	Phase relationships of these frequencies
	Acoustic envelope - changes in amplitude over time:
- Attack
- Decay
- Sustain
- Release
- *Look Up: Acoustic Envelope diagram*

Inverse Square Law - doubling the distance between the source of a sound and the pickup of the sound, will lower the direct signal level by 6dBSPL.

---
## Proper Gain Staging / Good Level Practices

- Noise Floor: low level noise produced by most electronic devices.
- Normal Operating Level: “typical”, “normal” or “standard” operating level *reference levels*
- Clipping / distortion
- Signal to Noise Ratio (S/N): higher is better
- Headroom: the difference between the Normal Operating Level and the level where distortion begins. Higher is better
- Dynamic Range: The difference in dB between the Noise Floor and the point of distortion.

- Amplitude can be measured in many ways…
	- Peak: the absolute peak of the waveform.
	- RMS/Avg: represents more the way humans judge loudness.

- Metering
	- Volume Units: Mechanical needle.
	- Bar-graph meter: emulates many types

- The Ear & Perception of Sound (Psychoacoustics)
	- Transducer: changes one form of energy into another.
	- The ear changes acoustic energy into the neural energy our brains understands.
	- Non-Linear Auditory Perception: What goes in is not always what comes out.
		- Ears produce Harmonic Distortion above certain SPLs
			- The production of harmonics that don’t exist in the original signal
		- Sensitivity changes with frequency & amplitude (Fletcher-Munson Graph)

		- Fletcher-Munson Equal Loudness Contours
			- Humans hear upper-mid frequencies better than highs & lows
			- Approx. 85dB is the linear sweet spot for mixing

		- Beats
			- Situation: 2 tones differ only slightly in frequency and approximately the same amplitude.
			- Effect: repetitive volume surges.
			- Cause: sum of frequencies when in phase & difference when out of phase.
			- Due to the ear’s inability to separate closely pitched notes.
			- Helpful for tuning - slow and stop when approach the same pitch.

		- Masking
			- Situation: Loud sounds and soft sounds - that are close in frequency.
			- Effect: Lout signal “prevents” the ear from hearing the softer sound.
			- Instruments that sound fine by themselves can be completely hidden or changed in character by louder instruments of similar timbre.

	- Perception of Direction
		- Inter-aural intensity differences
		- Inter-aural arrival time differences

		- Phantom Center & Panorama
			- Two speakers can simulate sound coming from any location between the speakers.
			- The exact same sound from both speakers will sound like it originates from center.
			- Panning changes perceived location by changing inter-aural intensity.
			- Panning can be used to combat masking.

	- Perception of Space
		- Direct Sound: determines source location, size, and true timbre.
		- Early Reflections: provides clues on reflectivity, size & nature of room, reflections from largest boundaries.
		- Reverberation (reverb): densely packed reflections, help determine distance from source, less highs &more apparent lows, often times use artificial reverband delay units to simulate different spaces.