**MADI stands for Multi-channel Audio Digital Interface**

MADI is an AES specification for digital interconnection between multitrack recorders and mixing consoles. It is an international standard (AES-10) offering 56 audio channels on a single coaxial cable or fiber-optic interface.

---

MADI supports serial digital transmission over coaxial cable or fibre-optic lines of 28, 56, 32, or 64 channels; and sampling rates to 96 kHz and beyond with an audio bit depth of up to 24 bits per channel.

Like AES3 and ADAT Lightpipe, it is a unidirectional interface from one sender to one receiver.

---

The original specification (AES10-1991) defined the MADI link as a 56 channel transport for linking large-format mixing consoles to digital multi-track recording devices. Large broadcast studios also adopted it for routing multi-channel audio throughout their facilities. The 2003 revision (AES10-2003) adds a 64 channel capability by removing vari-speed operation and supports 96 kHz sampling frequency with reduced channel capacity.The latest AES10-2008 standard includes minor clarifications and updates to correspond to the current AES3 standard.

MADI links use a transmission format similar to Fiber Distributed Data Interface (FDDI) networking. Since MADI is most often transmitted on copper links via 75 ohm coaxial cables, it more closely compares to the FDDI specification for copper-based links, called CDDI. AES10-2003 recommends using BNC connectors with coaxial cables and SC connectors with optic fibres. MADI over fibre can support a range of up to 2 km.

The basic data rate is 100 Mbit/s of data using 4B5B encoding to produce a 125 MHz physical baud rate. Unlike AES3, this clock is not synchronized to the audio sample rate, and the audio data payload is padded using JK sync symbols. Sync symbols may be inserted at any subframe boundary, and must occur at least once per frame. Though the standard disassociates the transmission clock from the audio sample rate, and thus requires a separate word clock connection to maintain synchronisation, some vendors do give the option of locking to parts of the transmission timing information for purposes of deriving a word clock.

The audio data is almost identical to the AES3 payload, though with more channels. Rather than letters, MADI assigns channel numbers from 0–63. Frame synchronization is provided by sync symbols outside the data itself, rather than an embedded preamble sequence, and the first four time slots of each sub-channel are encoded as normal data, used for sub-channel identification:

- Bit 0: Set to 1 to mark channel 0, the first channel in each frame
- Bit 1: Set to 1 to indicate that this channel is active (contains interesting data)
- Bit 2: notA/B channel marker, used to mark left (0) and right (1) channels. Generally, even channels are A and odd channels are B.
- Bit 3: Set to 1 to mark the beginning of a 192-sample data block