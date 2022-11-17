# Signal Processing
[*Build on Basic Audio Recording Additional signal flow principals*](/Sound/Basic%20Audio%20Recording/Advanced%20Signal%20Flow%20Principles.md)

## The Essential Elements of Mixing
The 2 most important aspects of signal processing are frequency and amplitude (the fundamentals of sound).

  
### Equalization (EQ) - A processing category that can be used to alter the frequency response characteristics of a signal. Boosts or attenuates frequency ranges in a signal.

- Filter Types:
	- Shelving: All frequencies above or below a certain point are amplified or attenuated by the same amount. Shelving filter are either on the low frequency or high frequency ends. There is no such thing as a mid shelf.
		- The most basic type of EQ. Treble/Bass (consumer audio).
		- Primary Controls:
			- Gain +/- (amount being done)
			- Frequency (where it’s being done)
	- Peaking
		- A range of frequencies around a point are boosted or attenuated.
		- “Center frequency” - the closer to the center, more boost/cut. Further away from the center, less boost/cut. (Bell curve)
		- The Bandwidth of the Peaking filter is known as “Q”. Q determines how wide or narrow the bell curve is. This determines the range of frequencies affected.
	- High/Low pass
		- A types of EQ that attenuates frequencies above or below a certain point.
		- “Cut off frequency” or “Corner frequency” - the point at which attenuation has begun and has reached -3dB.
		- Attenuation occurs in dB per octave. Amount is referred to as “Slope”. Attenuation is continuous; it never shelves. Usually 6, 12, 18 or 24dB per octave.
	- Band pass
		- Combined high/low pass filter.
	- Notch filter
		- Eliminates a very narrow band of frequencies, more than a peaking filter can do.

	- EQ’s may use a combination or all of these design types in one product.

- EQ Bands
	- Most EQ’s have the ability to affect more than one frequency at a time. Each with its own set of controls. Each frequency range is referred to as a “band”. Range from 2-Band, 3-Band, 4-Band, etc.

- Multi-Band EQ’s:
	- Parametric: Peaking and Shelving filters with full “parameter” controls are examples.
		- Controls for frequency, gain, Q and possibly slope.
		- Typically 3 or 4 bands.
		- Most common studio EQ.
	- Graphic: A type of Peaking EQ.
		- Center Frequency and Q are preset. Professional Graphic EQ’s generally have 25-36 bands, separated by approx. 1/3rd octave.

- Uses for EQ
	- Tone shaping.
	- Reducing unwanted sounds (leakage or noise (aspects of the sound that aren’t tone)).

### Dynamics - A Processing category that is used to alter the dynamic range of a signal. Increase/decrease dynamic range. Control volume peaks of a signal.

- “Downward” Compression
	- “regular” or “standard” compression. Reduces dynamic range. Applies gain reduction to loud signals, does nothing to soft signals.

- “Upward” Compression
	- Used far less often than “downward” Compression. Reduces the dynamic range by turning up the soft signals, does nothing to loud signals.

- Compression Parameters:
	- Threshold: Level at which the compressor begins working.
	- Ratio: Expresses the amount of gain reduction. Input signal : Output signal.
	- Attack: How quickly the processor reaches its final gain reduction to signals that have crossed the threshold. Also applies to all rising signals that are above the threshold.
	- Release: How quickly the processor returns to unity gain once the signal drops back below the threshold. Also applies to all falling signals that are above the threshold.
	- Attack & Release are usually expressed as a time unit (ms.) 
		- Not always user controllable. Sometimes the settings are pre-set in the unit or base architecture. Sometimes the settings are program dependent. “Auto” attack, “Auto” release.
	- Make-Up Gain: Post processing gain control.
		- Usually a manual adjustment, apply an amount that is equal but opposite to the average amount of gain reduction. Some compressors have “auto make-up gain”.
	- Knee - Controls how the processor reacts to signals as they approach the threshold.
		- Hard Knee - sudden onset of the compression ratio at the threshold level.
		- Soft Knee - onset of compression slowly increases as a signal approaches the threshold.
	- Peak vs RMS
		- Peak compressors will react to instantaneous peaks in the signal.
		- RMS compressors react only to changes in the average level of a signal.

- Limiting
	- Works like a compressor but with higher ratios. 10:1 and higher.
	- Soft Limiting vs Hard Limiting
		- Soft: lower thresholds, slower attack times
		- Hard: higher thresholds, faster attack times
	- Peak Limiters (Brick Wall Limiters)
		- High ratio and fast attack time
		- 20:1 up to Infinity:1
	- Output ceiling: set to -1dB or -2dB (digital cannot exceed 0dBFS (dB Full Scale))

- Expansion
	- An expander increases dynamic range by reducing the level of signals below the threshold.
	- Threshold, Attack and Release operate the same as in compression.
	- Range is the amount of gain reduction applied (dB)

- Gating
	- Operates like an expander.
	- Attempts to turn signals off when they fall below the threshold.
	- Gate is open when signal is loud enough to cross the threshold.
	- Gates are high ratio expanders.

- Dynamics Design (what happens in the dyn processor)
	- The input signal is split in two.
		- One signal goes to a variable gain amp. This is the signal we will hear at the output and which may have gain reduction applied.
		- One signal goes to the detection circuit (the Side-Chain/Key Input). This signal will determine if gain reduction is to be applied. We do not hear this signal unless we specifically access it.

	- The Side Chain
		- EQ’d/Filtered side chain
			- A side-chain signal can be tailored so that only certain frequency will control the gain reduction.
			- i.e. De-esser: Remove Sibilance
		- The side-chain can provide an alternative input source to the detection circuit of dynamics processors.
			- Signal A can control when gain reduction is applied to Signal B (the compressor).
			- Signal A can control when the gate opens on Signal B (EXP/GATE)
			- Key input - access to the side chain
			- Ducking, triggered gates, etc.

	- Stereo Linking
		- Stereo signals generally require that gain reduction be applied to both left and right sides equally. Otherwise the stereo image may shift.
		- Threshold detects a sum of the left and right signals.
		- Individual controls may still operate on the individual channels but the detection circuit is linked.
		- Some engineers prefer unlinked for width (experiment).

	- Multi-Band Compression
		- Works by splitting the signal into several different frequency ranges for individual processing. Signals are recombined at the output of the processor. Each frequency band is assigned its own processor.
		- Gives independent dynamics control over the different frequency ranges.

### Time Based Effects
- An effect category that can be used to alter and/or augment a signal based around delays and regeneration of signal over time.
- Often used to change perceived depth, dimension or character of sound. Can be used to add ambience to dry signals.
- The original sound is unchanged; the effect is being added.

- Delay
	- Incoming signal is temporarily held and replayed moments later.
	- Originally, tape machines were used. Later, other analog delay devices were developed. Later, digital “sampling”.
	- Basic features and controls
		- I/O controls
		- Delay time: the time between the original sound and its delay - or between each repeated delay - , usually in milliseconds.
		- Feedback: returning the delayed signal back into the input to create more repeats.
		- Mix or Balance percentage (plugins always at 100%).
		- Often basic H/LP Filters.
		- Modulation: the ability to change delay time (poss other parameters as well)
			- Rate: how fast will it change?
			- Depth: how much will it change?
			- Shape: what form will the change take?

	- Delay - 3 categories
		- Long: Greater than 35-50ms.
		- Delayed signal may be played back once or more than once.
		- Delayed signal can be processed (other filters, etc).

		- Medium/Short: Less than approx 50ms; delay cannot generally be heard as a discrete delay. The brain tends to fuse it with the original sound.
			- Result is an altered frequency response.
			- Constructive/Destructive interference when 2 signals are combined (delayed signal combined with the original).

		- Calculate Delay Times
			- By ear.
			- Tapping.
			- Use math.
			- Most DAWs or Plugins handle this in-house.

- Phasing and Flanging
	- When delay times fall below 10ms, a combing effect is created, add in small modulations and a sweeping comb filter effect is created.
	- Phasing - small modulations in delay time along with a phase inverted band pass filter.
	- Flanging - moderate to large shifts in delay time, across all frequencies.
	- Phasers are more specific while Flangers are more generalized.

- Doublers/ADT
	- Delay time in this range tends to create a doubling effect instead of comb filtering or discrete delays.
	- ADT - Automatic Double Tracking.
		- 20-50ms delay times *haas effect*
		- *Not a replacement for real double tracking*

- Some delay processors allow for more modulations than just delay time: Panning, Volume (tremolo), Pitch (Chorusing).

- Other Delay FX
	- Multi-tap delay
		- Multiple delay times in one effect.
		- Each delay time (tap) has its own set of controls.

	- Reverberation: A series of closely spaced and densely packed reflections. Aka a shit ton o’ delays.
		- 2 main components:
			- Early Reflections (ER)
			- Reverberations (Rev or Decay)
			- ER and Reverb mix with Direct Sound at the mic in live situations such as room mics. In a mixing environment, the Direct Sound is your dry signal feeding the stereo bus.
			- Use a Post Fader Send to feed the effect which creates ER and Rev. The effects return feeds Wet signal to the stereo bus to complete the illusion.
		- Reverb Types:
			- Acoustic Reverb: The sound of the recording space itself.
			- Reverb Chamber: can be done live while recording or added later using Aux Send/Return.
			- Mechanical Reverbs:
				- Plate Reverb: Metal plate that gets vibrated and transducers pick up that vibration.
				- Spring Reverb: Injects sound into metal springs and letting them reverberate. Tend to sound “bouncy” but can also be “ringy” and feedback into themselves.
				- Hall Reverb: A hall reverb is usually good for adding 3-dimensional ambiance to the mix. They tend to fill out the back of the mix, adding depth without crowding the foreground.
				- Room Reverb: Good for adding realism to instruments that have very close mic’ing positioning or DI. The reverb is designed to give the listener the sense that the instrument is being played in an actual acoustic space.
				- Reverse Reverb: The sound of the reverb running backwards. Instead of starting with the original sound and then gradually dying out, it starts softly and gradually gets louder until the original sound is heard.
				- Gated Reverb: Setup by putting a noise gate after the reverb in order to purposefully cut off the reverb.
				- Algorithmic Reverb: A kind of reverb device that is calculated in real time using DSP code. These usually have many perimeters, making them flexible and versatile.
				- Convolution Reverb: Uses samples of real-life acoustic spaces. But, often, have limited ability to modify the reverb sound.
		- Reverb Parameters
			- ER - the first reflections
			- Rev Time (Decal) in ms
			- Pre Delay - delay inserted before anything happens
			- Type
			- Room size
			- Damping
			- Pre verb EQ (hi/lo)
			- Diffusion
			- Density
			- Post verb EQ