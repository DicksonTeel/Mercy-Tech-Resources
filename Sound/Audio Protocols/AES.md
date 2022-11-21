AES3 is a standard for the exchange of digital audio signals between professional audio devices. An AES3 signal can carry two channels of pulse-code-modulated digital audio over several transmission media including balanced lines, unbalanced lines, and optical fiber.

AES3 was jointly developed by the Audio Engineering Society (AES) and the European Broadcasting Union (EBU) and so is also known as AES/EBU. The standard was first published in 1985 and was revised in 1992 and 2003. AES3 has been incorporated into the International Electrotechnical Commission's standard IEC 60958, and is available in a consumer-grade variant known as [S/PDIF](/Sound/Audio%20Protocols/SPDIF.md).

---

Type I connections use balanced, three-conductor, 110-ohm twisted pair cabling with XLR connectors. Type I connections are most often used in professional installations and are considered the standard connector for AES3.

Type II defines an unbalanced electrical or optical interface for consumer electronics applications. The precursor of the IEC 60958 Type II specification was the Sony/Philips Digital Interface, or S/PDIF. Both were based on the original AES/EBU work. S/PDIF and AES3 are interchangeable at the protocol level, but at the physical level, they specify different electrical signalling levels and impedances, which may be significant in some applications.

AES/EBU signals can also be run using unbalanced BNC connectors a with a 75-ohm coaxial cable. The unbalanced version has a very long transmission distance as opposed to the 150 meters maximum for the balanced version. The AES-3id standard defines a 75-ohm BNC electrical variant of AES3. This uses the same cabling, patching and infrastructure as analogue or digital video, and is thus common in the broadcast industry.

---

AES3 was designed primarily to support stereo PCM encoded audio in either DAT format at 48 kHz or CD format at 44.1 kHz. No attempt was made to use a carrier able to support both rates; instead, AES3 allows the data to be run at any rate, and encoding the clock and the data together using biphase mark code (BMC).

Each bit occupies one time slot. Each audio sample (of up to 24 bits) is combined with four flag bits and a synchronisation preamble which is four time slots long to make a subframe of 32 time slots.

---

SMPTE timecode data can be embedded within AES3 signals. It can be used for synchronization and for logging and identifying audio content.