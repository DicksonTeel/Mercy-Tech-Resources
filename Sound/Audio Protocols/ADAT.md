The ADAT Lightpipe, officially the **ADAT Optical Interface**, is a standard for the transfer of digital audio between equipment. It was originally developed by Alesis but has since become widely accepted, with many third party hardware manufacturers including Lightpipe interfaces on their equipment. The protocol has become so popular that the term ADAT is now often used to refer to the transfer standard rather than to the Alesis Digital Audio Tape itself.

Lightpipe uses the same connection hardware as S/PDIF: fiber optic cables (hence its name) to carry data, with Toslink connectors and optical transceivers at either end. However, the data streams of the two protocols are incompatible. S/PDIF is mostly used for transferring stereo or multi-channel surround sound audio, whereas the ADAT optical interface supports up to 8 audio channels at 48 kHz, 24 bit.

---

Lightpipe can carry eight channels of uncompressed digital audio at 24 bit resolution at 48,000 samples or four channels at 96,000 samples per second. Initially used for the transfer of digital audio between ADATs, the protocol was designed with future improvements in mind. All Lightpipe signals are transmitted at 24 bit resolution, no matter what the depth of the audio; information is contained within the *Most Significant Bits* and the rest of the bits remain a string of zeros. For example, if a 16 bit signal is sent via Lightpipe, the first sixteen bits contain the audio information while the other eight are simply occupied by zeros. The receiving device ignores information it cannot process. For example, a 20 bit signal going from a Type II ADAT to a Type I (which only operates at 16 bits) will simply ignore the bits below the sixteen MSBs.

Higher sample rates can be accommodated with a reduced number of channels. While the original ADAT machines did not support this, the Lightpipe format was modified using bit-splitting techniques by the company Sonorus. Known as S/MUX (short for 'sample multiplexing'), this connection allows 4 channels at up to 96 kHz, or two channels at up to 192 kHz, on one optical cable. Most manufacturers implementing ADAT Lightpipe now support this S/MUX interface extension.

Light carrying the data signal through the Lightpipe is turned into an electronic data stream going to an IC chip commonly referred to at Alesis as "the 1-K chip". From there the audio data frame is routed to processing ICs.

With an ADAT Lightpipe and an ADAT controller linking up to four ADATs using CAT5 cables with RJ-connectors and SMPTE Time Code, you could synchronize four 8-track ADATs together for a total of 32 simultaneous synchronized channel tracks of 16 or 20 bit audio data. 24 bit came later with the HD24 hard disk recorder in early 2001, which also made use of Lightpipe capabilities.

---

In order to fit 8 channels within the bandwidth limits of the standard TOSLINK transceiver modules, the bitstream is not biphase mark coded like S/PDIF. Instead, NRZI coding is used, where a 0 bit indicates no transition and a 1 bit is a transition. 8 audio samples at 24 bits per sample plus 4 user bits (196 bits total) are sent in groups of 4 data bits followed by a 1 bit to force a transition. This totals 196×5/4 = 245 bits. 10 consecutive 0 bits followed by a 1 bit provide frame synchronization.

One frame is sent at the desired sample rate, for a bit rate of 256×48 kHz = 12.288 Mbit/s. This is twice the baud rate used by S/PDIF (3.072 Mbit/s, doubled by biphase coding to 6.144 Mbaud), but still within the specified 15 Mbaud capacity of the popular TOTX147 /TORX147 TOSLINK transceivers.

User data bit allocations:
- User bit 0 is designated for Timecode transport
- User bit 1 is designated for MIDI data transport
- User bit 2 is designated for S/Mux indication (96 kHz sample rate mode)
- User bit 3 is reserved and set to 0

The transmission speed of the user bits is equal to the sampling rate (e.g. 48,000 bits per second)

---
An advantage of ADAT to other comperable protocols is that the lightpipe is "hot-pluggable", which means devices do not need to be turned off for plugging in or unplugging (although it is advisable to mute the receiving equipment, since there will be a large signal spike when the connection is made). The optical connect avoids ground-loops, which can be troublesome in larger installations, and will not transfer any harmful electrical spikes from one device to the next.