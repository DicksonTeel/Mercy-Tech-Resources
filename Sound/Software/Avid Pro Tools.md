Link to Avid Pro Tools: [Avid Pro Tools](https://www.avid.com/pro-tools)

Link to Pro Tools Support: [Pro Tools Learn & Support](https://www.avid.com/pro-tools/learn-and-support)

Pro Tools is a digital audio workstation (DAW) developed and released by Avid Technology (formerly Digidesign) for
Microsoft Windows and macOS. It is used for music creation and production, sound for picture (sound design, audio
post-production and mixing) and, more generally, sound recording, editing, and mastering processes.

Pro Tools operates both as standalone software and in conjunction with a range of external analog-to-digital converters
and PCIe cards with on-board digital signal processors (DSP). The DSP is used to provide additional processing power to
the host computer for processing real-time effects, such as reverb, equalization, and compression and to obtain lower
latency audio performance. Like all digital audio workstation software, Pro Tools can perform the functions of a
multitrack tape recorder and a mixing console along with additional features that can only be performed in the digital
domain, such as non-linear and non-destructive editing (most of the audio handling is done without overwriting the
source files), track compositing with multiple playlists, time compression and expansion, pitch shifting, and
faster-than-real-time mixdown.

Audio, MIDI, and video tracks are graphically represented on a timeline. Audio effects, virtual instruments, and
hardware emulators—such as microphone preamps or guitar amplifiers—can be added, adjusted, and processed in real-time in
a virtual mixer. 16-bit, 24-bit, and 32-bit float audio bit depths at sample rates up to 192 kHz are supported. Pro
Tools supports mixed bit depths and audio formats in a session: BWF/WAV (including WAVE Extensible, RF64 and BW64) and
AIFF. It imports and exports MOV video files and ADM BWF files (audio files with Dolby Atmos metadata); it also
imports MXF, ACID and REX files and the lossy formats MP3, AAC, M4A, and audio from video files (MOV, MP4, M4V). The
legacy SDII format was dropped with Pro Tools 10, although SDII conversion is still possible on macOS.

Pro Tools has incorporated video editing capabilities, so users can import and manipulate high-definition video file
formats such as XDCAM, MJPG-A, PhotoJPG, DV25, QuickTime, and more. It features time code, tempo maps, elastic audio,
and automation; supports mixing in surround sound, Dolby Atmos and VR sound using Ambisonics.

The Pro Tools TDM mix engine, supported until 2011 with version 10, employed 24-bit fixed-point arithmetic for plug-in
processing and 48-bit for mixing. Current HDX hardware systems, HD Native and native systems use 32-bit floating-point
resolution for plug-ins and 64-bit floating-point summing. The software and the audio engine were adapted to 64-bit
architecture from version 11.

In 2022, Avid switched Pro Tools from a perpetual license to a subscription model. New users have to choose between
three new plans: Pro Tools Artist, which costs $9.99 per month or $99 per year; Pro Tools Studio, which costs $39.99 per
month or $299 per year; and Pro Tools Flex, which costs $99.99 per month or $999 per year. Later in 2022, Avid
launched a free version: Pro Tools Intro.

## The beginnings: Digidrums (1983–1985)

Pro Tools was developed by UC Berkeley graduates Evan Brooks, who majored in electrical engineering and computer
science, and Peter Gotcher.

In 1983, the two friends, sharing an interest in music and electronic and software engineering, decided to study the
memory mapping of the newly released E-mu Drumulator drum machine to create EPROM sound replacement chips. The
Drumulator was quite popular at that time, although it was limited to its built-in samples.

They started selling the upgrade chips one year later under their new Digidrums label. Five different upgrade chips
were available, offering different alternate drum styles. The chips, easily switchable with the original ones, enjoyed
remarkable success between the Drumulator users, selling 60,000 units overall.

## Digidesign Sound Designer (1985–1989)

When Apple released its first Macintosh computer in 1984, the pair thought to design a more functional and flexible
solution which could take advantage of a graphical interface. In collaboration with E-Mu, they developed a Mac-based
visual sample editing system for the Emulator II keyboard, called Sound Designer, released under the Digidesign
brand and inspired by the interface of the Fairlight CMI. This system, the first ancestor of Pro Tools, was
released in 1985 at the price of US$995.

Brooks and Gotcher rapidly ported Sound Designer to many other sampling keyboards, such as E-mu Emax, Akai S900,
Sequential Prophet 2000, Korg DSS-1, and Ensoniq Mirage. Thanks to the universal file specification subsequently
developed by Brooks with version 1.5, Sound Designer files could be transferred via MIDI between sampling keyboards
of different manufacturers. This universal file specification, along with the printed source code to a 68000
assembly language interrupt-driven MIDI driver, was distributed through Macintosh MIDI interface manufacturer
Assimilation, which manufactured the first MIDI interface for the Mac in 1985.

Starting from the same year, a dial-up service provided by Beaverton Digital Systems, called MacMusic, allowed Sound
Designer users to download and install the entire Emulator II sound library to other less expensive samplers: sample
libraries could be shared across different manufacturers platforms without copyright infringement. MacMusic contributed
to Sound Designer's success by leveraging both the universal file format and developing the first online sample file
download site globally, many years before the World Wide Web use soared. The service used 2400-baud modems and 100 MB of
disk space with Red Ryder host on a 1 MB Macintosh Plus.

With the release of Apple Macintosh II in 1987, which provided card slots, a hard disk, and more capable memory, Brooks
and Gotcher saw the possibility to evolve Sound Designer into a featured digital audio workstation. They discussed with
E-mu the opportunity of using the Emulator III as a platform for their updated software, but E-mu rejected this offer.
Therefore, they decided to design both the software and the hardware autonomously. Motorola, which was working on its
56K series of digital signal processors, invited the two to participate in its development. Brooks designed a circuit
board for the processor, then developed the software to make it work with Sound Designer. A beta version of the DSP was
ready by December 1988.

## Digidesign Sound Tools and Sound Designer II software (1989–1990)

The combination of the hardware and the software was called Sound Tools. Advertised as the "first tapeless studio",
it was presented on January 20, 1989, at the NAMM annual convention. The system relied on a NuBus card called Sound
Accelerator, equipped with one Motorola 56001 processor. The card provided 16-bit playback and 44.1/48 kHz recording
through a two-channel A/D converter (AD In), while the DSP handled signal processing, which included a ten-band graphic
equalizer, a parametric equalizer, time stretching with pitch preservation, fade-in/fade-out envelopes, and
crossfades ("merging") between two sound files.

Sound Tools was bundled with Sound Designer II software, which was, at this time, a simple mono or stereo audio editor
running on Mac SE or Mac II; digital audio acquisition from DAT was also possible. A two-channel digital interface (
DAT-I/O) with AES/EBU and S/PDIF connections was made available later in 1989, while the Pro I/O interface came out in
1990 with 18-bit converters.

The file format used by Sound Designer II (SDII) became eventually a standard for digital audio file exchange until the
WAV file format took over a decade later. Since audio streaming and non-destructive editing were performed on hard
drives, the software was still limited by their performance; densely edited tracks could cause glitches. However,
the rapidly evolving computer technology allowed developments towards a multi-track sequencer.

## Deck, Pro Tools, Sound Tools II and Pro Tools II (1990–1994)

The core engine and much of the user interface of the first iteration of Pro Tools was based on Deck. The software,
published in 1990, was the first multi-track digital recorder based on a personal computer. It was developed by OSC, a
small San Francisco company founded the same year, in conjunction with Digidesign and ran on Digidesign's hardware.
Deck could run four audio tracks with automation; MIDI sequencing was possible during playback and record, and one
effect combination could be assigned to each audio track (2-band parametric equalizer, 1-band EQ with delay, 1-band EQ
with chorus, delay with chorus).

The first Pro Tools system was launched on June 5, 1991. It was based on an adapted version of Deck (ProDeck) along with
Digidesign's new editing software, ProEdit, created by Mark Jeffery; Sound Designer II was still supplied for
two-channel editing. Pro Tools relied on Digidesign's Audiomedia card, mounting one Motorola 56001 processor
with a clock rate of 22.58 MHz and offering two analog and two digital channels of I/O, and on the Sound Accelerator
card. External synchronization with audio and video tape machines was possible with SMPTE timecode and the Video Slave
drivers. The complete system was selling for US$6,000.

Sound Tools II was launched in 1992 with a new DSP card. Two interfaces were also released: Pro Master 20, providing
20-bit A/D conversion, and Audiomedia II, with improved digital converters and one Motorola 56001 processor running
at 33.86 MHz.

In 1993, Josh Rosen, Mats Myrberg and John Dalton, the OSC's engineers who developed Deck, split from Digidesign to
focus on releasing lower-cost multi-track software that would run on computers with no additional hardware. This
software was known as Session (for stereo-only audio cards) and Session 8 (for multichannel audio interfaces) and was
selling for US$399.

Peter Gotcher felt that the software needed a significant rewrite. Pro Tools II, the first software release fully
developed by Digidesign, followed in the same year and addressed its predecessor's weaknesses. The editor and the
mixer were merged into a single Pro Tools application that utilized the Digidesign Audio Engine (DAE) created by Peter
Richert. DAE was also provided as a separate application to favor hardware support from third-party developers, enabling
the use of Pro Tools hardware and plug-ins on other DAWs. Selling more than 8,000 systems worldwide, Pro Tools
II became the best-selling digital audio workstation.

## Pro Tools II TDM: 16 tracks and real-time plug-ins (1994)

In 1994, Pro Tools 2.5 implemented Digidesign's newly developed time-division multiplexing technology, which allowed
routing of multiple digital audio streams between DSP cards. With TDM, up to four NuBus cards could be linked, obtaining
a 16-track system, while multiple DSP-based plug-ins could be run simultaneously and in real-time. The wider
bandwidth required to run the larger number of tracks was achieved with a SCSI expansion card developed by Grey Matter
Response, called System Accelerator.

In the same year, Digidesign announced that it merged into the American multimedia company Avid, developer of the
digital video editing platform Media Composer and one of Digidesign's major customers (25% of Sound Accelerator and
Audiomedia cards produced was being bought by Avid). The operation was finalized in 1995.

## Pro Tools III: 48 tracks, DSP Farm cards and switch to PCI cards (1995–1997)

With a redesigned Disk I/O card, Pro Tools III was able to provide 16 tracks with a single NuBus card; the system
could be expanded using TDM to up to three Disk I/O cards, achieving 48 tracks. DSP Farm cards were introduced to
increase the processing power needed for a more extensive real-time audio processing; each card was equipped with three
Motorola 56001 chips running at 40 MHz. Multiple DSP cards could be added for additional processing power; each card
could handle the playback of 16 tracks. A dedicated SCSI card was still required to provide the required bandwidth
to support multiple-card systems.

Along with Pro Tools III, Digidesign launched the 888 interface, with eight channels of analog and digital I/O, and the
cheaper 882 interface. The Session 8 system included a control surface with eight faders. A series of TDM
plug-ins were bundled with the software, including dynamics processing, EQ, delay, modulation, and reverb.

In 1996, following Apple's decision to drop NuBus in favor of PCI bus, Digidesign added PCI support with Pro Tools 3.21.
The PCI version of the Disk I/O card incorporated a high-speed SCSI along with DSP chips, while the upgraded DSP
Farm PCI card included four Motorola 56002 chips running at 66 MHz.

This change of architecture allowed the convergence of Macintosh computers with Intel-based PCs, for which PCI had
become the standard internal communication bus. With the PCI version of Digidesign's Audiomedia card in 1997 (
Audiomedia III), Sound Tools and Pro Tools could be run on Windows platforms for the first time.

## 24-bit audio and surround mixing: Pro Tools | 24 and Pro Tools | 24 MIX (1997–2002)

With the release of Pro Tools | 24 in 1997, Digidesign introduced a new 24-bit interface (the 888|24) and a new PCI
card (the d24). The d24 relied on Motorola 56301 processors, offering increased processing power and 24 tracks of 24-bit
audio (later increased to 32 tracks with a DAE software update). A SCSI accelerator was required to keep up with the
increased data throughput. Digidesign dropped its proprietary SCSI controller in favor of commercially available
ones.

64 tracks with dual d24 support were introduced with Pro Tools 4.1.1 in 1998, while the updated Pro Tools | 24 MIX
system provided three times more DSP power with the MIX Core DSP cards. MIXplus systems combined a MIX Core with a MIX
Farm, obtaining a performance increase of 700% compared to a Pro Tools | 24 system.

Pro Tools 5 saw two substantial software developments: extended MIDI functionality and integration in 1999 (an editable
piano-roll view in the editor; MIDI automation, quantize and transpose) and the introduction of surround sound
mixing and multichannel plug-ins—up to the 7.1 format—with Pro Tools TDM 5.1 in 2001.

The migration from traditional, tape-based analog studio technology to the Pro Tools platform took place within the
industry: Ricky Martin's "Livin' la Vida Loca" (1999) was the first Billboard Hot 100 number-one single to be
recorded, edited, and mixed entirely within the Pro Tools environment, allowing a more meticulous and effortless
editing workflow (especially on vocals).

While consolidating its presence in professional studios, Digidesign began to target the mid-range consumer market in
1999 by introducing the Digi001 bundle, consisting of a rack-mount audio interface with eight inputs and outputs with
24-bit, 44.1/48 kHz capability and MIDI connections. The package was distributed with Pro Tools LE, a specific version
of the software without DSP support, limited to 24 mixing tracks.

High-resolution audio and consolidation of digital recording and mixing: Pro Tools | HD (2002–2011)
Following the launch of Mac OS X operating system in 2001, Digidesign made a substantial redesign of Pro Tools hardware
and software. Pro Tools | HD was launched in 2002, replacing the Pro Tools | 24 system and relying on a new range of DSP
cards (HD Core and HD Process, replacing MIX Core and MIX Farm), new interfaces running at up to 192 kHz or 96 kHz
sample rates (HD 192 and 96, replacing 888 and 882), along with an updated version of the software (Pro Tools 6) with
new features and a redesigned GUI, developed for OS X and Windows XP. Two HD interfaces could be linked together for
increased I/O through a proprietary connection. The base system was selling for US$12,000, while the full system was
selling for US$20,000.

Both HD Core and Process cards mounted nine Motorola 56361 chips running at 100 MHz, each providing 25% more processing
power than the Motorola 56301 chips mounted on MIX cards; this translated to about twice the power for a single card. A
system could combine one HD Core card with up to two HD Process cards, supporting playback for 96/48/12 tracks at
48/96/192 kHz sample rates (with a single HD Core card installed) and 128/64/24 tracks at 48/96/192 kHz sample rates (
with one or two HD Process cards).

When Apple changed the expansion slot architecture of the Mac G5 to PCI Express, Digidesign launched a line of PCIe DSP
cards that both adopted the new card slot format and slightly changed the combination of chips. HD Process cards were
replaced with HD Accel, each mounting nine Motorola 56321 chips running at 200 MHz and each providing twice the power
than an HD Process card; track count for systems mounting an HD Accel was extended to 192/96/36 tracks at 48/96/192 kHz
sample rates. The use of PCI Express connection reduced round-trip delay time, while DSP audio processing allowed
the use of smaller hardware buffer sizes during recording, assuring stable performance with extremely low latency.

Pro Tools, offering a solid and reliable alternative to analog recording and mixing, eventually became a standard in
professional studios throughout the decade, while editing features such as Beat Detective (introduced with Pro Tools 5.1
in 2001) and Elastic Audio (introduced with Pro Tools 7.4 in 2007) redefined the workflow adopted in
contemporary music production.

Other software milestones were background tasks processing (such as fade rendering, file conversion or relinking),
real-time insertion of TDM plug-ins during playback, and a browser/database environment introduced with Pro Tools 6 in
2003; Automatic plug-in Delay Compensation (ADC), introduced with Pro Tools 6.4 in 2004 and only available with TDM
systems with HD Accel; a new implementation of RTAS with multi-threading support and improved performance, Region
groups, Instrument tracks, and real-time MIDI processing, introduced with Pro Tools 7 in 2006; VCA and volume trim,
introduced with Pro Tools 7.2 in 2006; support for ten track inserts, MIDI Editor, and MIDI Score, introduced with
Pro Tools 8 in 2009.

Pro Tools | MIX hardware support was dropped with version 6.4.1.

## Native systems: Pro Tools LE and Pro Tools M-Powered

Pro Tools LE, first introduced and distributed in 1999 with the Digi 001 interface, was a specific Pro Tools version
in which the signal processing entirely relied on the host CPU. The software required a Digidesign interface to run,
which acted as a copy-protection mechanism for the software. Mbox was the entry-level range of the available interface;
Digi 001 and Digi 002/003, which also provided a control surface, were the upper range. The Eleven Rack also ran on Pro
Tools LE, included in-box DSP processing via an FPGA chip, offloading guitar amp/speaker emulation, and guitar effects
plug-in processing to the interface, allowing them to run without taxing the host system.

Pro Tools LE shared the same interface of Pro Tools HD but had a smaller track count (24 tracks with Pro Tools 5,
extended to 32 tracks with Pro Tools 6 and 48 tracks with Pro Tools 8) and supported a maximum sample rate of 96
kHz (depending on the interface used). Some advanced software features, such as Automatic Delay Compensation,
surround mixing, multi-track Beat Detective, OMF/AAF support, and SMPTE Timecode, were omitted. Some of them, as well as
support for 48 tracks/96 voices (extended to 64 tracks/128 voices with Pro Tools 8) and additional plug-ins, were made
available through an expansion package called "Music Production Toolkit". The "Complete Production Toolkit",
introduced with Pro Tools 8, added support for surround mixing and 128 tracks (while the system was still limited to 128
voices).

With the acquisition of M-Audio in 2004–2005, Digidesign released a specific variant of Pro Tools, called M-Powered,
which was equivalent to Pro Tools LE and could be run with M-Audio interfaces.

The Pro Tools LE/M-Powered line was discontinued with the release of Pro Tools 9.

## Hardware-independent native systems: Pro Tools 9

Pro Tools 9, released in November 2010, dropped the requirement of proprietary hardware to run the software. Any audio
device could be used through Core Audio on macOS or the ASIO driver on a Windows. Core Audio allowed device aggregation,
enabling using of more than one interface simultaneously. Some Pro Tools HD software features, such as automatic plug-in
delay compensation, OMF/AAF file import, Timecode ruler, and multi-track Beat Detective, were included in the standard
version of Pro Tools 9.

When operating on a machine containing one or more HD Core, Accel, or Native cards, the software ran as Pro Tools HD
with the complete HD feature set. In all other cases, it ran as Pro Tools 9 standard, with a smaller track count and
some advanced features turned off.

## Advanced Instrument Research (AIR): built-in virtual instruments and plug-ins

In response to Apple's decision to include Emagic's complete line of virtual instruments in Logic Pro in 2004 and
following Avid's acquisition of German virtual instruments developer Wizoo in 2005, Pro Tools 8 was supplied with its
first built-in virtual instruments library, the AIR Creative Collection, as well as with some new plug-ins, to make it
more appealing for music production. An expansion was also available, called AIR Complete Collection.

## List of AIR Virtual Instruments

Pro Tools | HDX (2011–present)
In October 2011, Avid introduced Pro Tools 10 and a new series of DSP PCIe cards named HDX. Each card mounted 18 DSP
processors, manufactured by Texas Instruments, allowing an increased computational precision (32-bit floating-point
resolution for audio processing and 64-bit floating-point summing, versus the previous 24-bit and 48-bit fixed-point
resolution of the TDM engine), thus improving dynamic range performance. Signal processing could be run on the
embedded DSP, providing additional computational power and enabling near zero-latency for DSP-reliant plug-ins. Two FPGA
chips handled track playback, monitoring, and internal routing, providing a lower round trip latency.

A second line of PCIe cards, called HD Native, provided low latency with a single FPGA chip but did not mount DSP (audio
processing relied on the host system's CPU). Round trip latency at 96 kHz was 0.7 ms for HDX and 1.7 ms for HD
Native (with a 64-sample buffer).

To maintain performance consistency, HDX products were specified with a fixed maximum number of voices (each voice
representing a monophonic channel). Each HDX card enabled 256 simultaneous voices at 44.1/48 kHz; voice count halved
when the sample rate doubled (128 voices at 88.2/96 kHz, 64 voices at 176.4/192 kHz). Up to three HDX cards could be
installed on a single system for a maximum of 768/384/192 total voices and for increased processing power. On Native
systems, voice count was limited to 96/48/24 voices with the standard version of Pro Tools and 256/128/64 voices with
Pro Tools HD software.

With Pro Tools 10, Avid deployed a new plug-in format for both Native and HDX systems called AAX (an acronym for Avid
Audio eXtension). AAX Native replaced RTAS plug-ins and AAX DSP, a specific format running on HDX systems, replaced
TDM plug-ins. AAX was developed to provide the future implementation of 64-bit plug-ins, although 32-bit versions of AAX
were still used in Pro Tools 10. TDM support was dropped with HDX, while Pro Tools 10 would be the final release for
Pro Tools | HD Process and Accel systems.

Notable software features introduced with Pro Tools 10 were editable clip-based gain automation (Clip gain), the ability
to load the session's audio data into RAM to improve transport responsiveness (Disk caching), quadrupled Automatic Delay
Compensation length, audio fades processed in real-time, timeline length extended to 24 hours, support for 32-bit float
audio and mixed audio formats within the session, and the addition of Avid Channel Strip plug-in (based on Euphonix
System 5 console's channel strip, following Avid's acquisition of Euphonix in 2010).

## Switch to 64-bit architecture (2013)

Pro Tools 11, released in June 2013, switched from 32-bit to 64-bit software architecture with new audio and video
engines, enabling the application and plug-ins to fully take advantage of system memory. The new audio engine (AAE)
introduced support of offline bouncing and simultaneous mixdowns multiple sources; dynamic plug-in processing allowed to
reduce CPU usage when active native plug-ins do not receive any input. Two separate buffers were used for playback and
for monitoring of record-enabled or input-monitored tracks. The new video engine (AVE) improved performance and handling
of multiple CPU cores.

Support for HD Accel systems, legacy HD interfaces, TDM and 32-bit AAX plug-ins was dropped due to their incompatibility
with 64-bit architecture. A free starter edition providing the essential features of Pro Tools, called "First", was
launched in 2015 and discontinued in December 2021 for being "unviable to continue on a technical level".

## Editions (per 2022)

Pro Tools software is available in three subscription-based paid versions (Artist, Studio and Ultimate) and one free
version (Intro).

Before 2022, two different perpetual licenses could be purchased: a standard edition for US$599 (informally called "
Vanilla"), which provided all the key features for audio mixing and post-production, and a complete edition for
US$2599 (officially called "Ultimate" and known as "HD" between 2002 and 2018), which unlocked functionality for
advanced workflows and a higher track count.