## Summary
**High-Definition Multimedia Interface** (HDMI) is a proprietary audio/video interface for transmitting uncompressed video data and compressed or uncompressed digital audio data from an HDMI-compliant source device, such as a display controller, to a compatible computer monitor, video projector, digital television, or digital audio device. HDMI is a digital replacement for analog video standards.

HDMI implements the EIA/CEA-861 standards, which define video formats and waveforms, transport of compressed and uncompressed LPCM audio, auxiliary data, and implementations of the VESA EDID. CEA-861 signals carried by HDMI are electrically compatible with the CEA-861 signals used by the Digital Visual Interface (DVI). No signal conversion is necessary, nor is there a loss of video quality when a DVI-to-HDMI adapter is used. The Consumer Electronics Control (CEC) capability allows HDMI devices to control each other when necessary and allows the user to operate multiple devices with one handheld remote control device.

Several versions of HDMI have been developed and deployed since the initial release of the technology, occasionally introducing new connectors with smaller form factors, but all versions still use the same basic pinout and are compatible with all connector types and cables. Other than improved audio and video capacity, performance, resolution and color spaces, newer versions have optional advanced features such as 3D, Ethernet data connection, and CEC extensions.

## Specifications

### Audio/Video
HDMI uses the Consumer Technology Association/Electronic Industries Alliance 861 standards. HDMI 1.0 to HDMI 1.2a uses the EIA/CEA-861-B video standard, HDMI 1.3 uses the CEA-861-D video standard, and HDMI 1.4 uses the CEA-861-E video standard. The CEA-861-E document defines "video formats and waveforms; colorimetry and quantization; transport of compressed and uncompressed LPCM audio; carriage of auxiliary data; and implementations of the Video Electronics Standards Association (VESA) Enhanced Extended Display Identification Data Standard (E-EDID)". On July 15, 2013, the CEA announced the publication of CEA-861-F, a standard that can be used by video interfaces such as DVI, HDMI, and LVDS. CEA-861-F adds the ability to transmit several Ultra HD video formats and additional color spaces.

To ensure baseline compatibility between different HDMI sources and displays (as well as backward compatibility with the electrically compatible DVI standard) all HDMI devices must implement the sRGB color space at 8 bits per component. Ability to use the Y′CBCR color space and higher color depths ("deep color") is optional. HDMI permits sRGB 4:4:4 chroma subsampling (8–16 bits per component), xvYCC 4:4:4 chroma subsampling (8–16 bits per component), Y′CBCR 4:4:4 chroma subsampling (8–16 bits per component), or Y′CBCR 4:2:2 chroma subsampling (8–12 bits per component). The color spaces that can be used by HDMI are ITU-R BT.601, ITU-R BT.709-5 and IEC 61966-2-4.

For digital audio, if an HDMI device has audio, it is required to implement the baseline format: stereo (uncompressed) PCM. Other formats are optional, with HDMI allowing up to 8 channels of uncompressed audio at sample sizes of 16 bits, 20 bits, or 24 bits, with sample rates of 32 kHz, 44.1 kHz, 48 kHz, 88.2 kHz, 96 kHz, 176.4 kHz, or 192 kHz. HDMI also carries any IEC 61937-compliant compressed audio stream, such as Dolby Digital and DTS, and up to 8 channels of one-bit DSD audio (used on Super Audio CDs) at rates up to four times that of Super Audio CD. With version 1.3, HDMI allows lossless compressed audio streams Dolby TrueHD and DTS-HD Master Audio. As with the Y′CBCR video, audio capability is optional. Audio return channel (ARC) is a feature introduced in the HDMI 1.4 standard. "Return" refers to the case where the audio comes from the TV and can be sent "upstream" to the AV receiver using the HDMI cable connected to the AV receiver. An example given on the HDMI website is that a TV that directly receives a terrestrial/satellite broadcast, or has a video source built in, sends the audio "upstream" to the AV receiver.

The HDMI standard was not designed to pass closed caption data (for example, subtitles) to the television for decoding. As such, any closed caption stream must be decoded and included as an image in the video stream(s) prior to transmission over an HDMI cable to appear on the DTV. This limits the caption style (even for digital captions) to only that decoded at the source prior to HDMI transmission. This also prevents closed captions when transmission over HDMI is required for upconversion. For example, a DVD player that sends an upscaled 720p/1080i format via HDMI to an HDTV has no way to pass Closed Captioning data so that the HDTV can decode it, as there is no line 21 VBI in that format.

### Communication Channels
HDMI has three physically separate communication channels, which are the DDC, TMDS and the optional CEC. HDMI 1.4 added ARC and HEC.

#### Display Data Channel (DDC)
The Display Data Channel (DDC) is a communication channel based on the I2C bus specification. HDMI specifically requires the device implement the Enhanced Display Data Channel (E-DDC), which is used by the HDMI source device to read the E-EDID data from the HDMI sink device to learn what audio/video formats it can take. HDMI requires that the E-DDC implement I2C standard mode speed (100 kbit/s) and allows it to optionally implement fast mode speed (400 kbit/s). 

The DDC channel is actively used for High-bandwidth Digital Content Protection (HDCP).

#### Transition-minimized differential signaling (TMDS)
Transition-minimized differential signaling (TMDS) on HDMI interleaves video, audio and auxiliary data using three different packet types, called the video data period, the data island period and the control period. During the video data period, the pixels of an active video line are transmitted. During the data island period (which occurs during the horizontal and vertical blanking intervals), audio and auxiliary data are transmitted within a series of packets. The control period occurs between video and data island periods.

Both HDMI and DVI use TMDS to send 10-bit characters that are encoded using 8b/10b encoding that differs from the original IBM form for the video data period and 2b/10b encoding for the control period. HDMI adds the ability to send audio and auxiliary data using 4b/10b encoding for the data island period. Each data island period is 32 pixels in size and contains a 32-bit packet header, which includes 8 bits of BCH ECC parity data for error correction and describes the contents of the packet. Each packet contains four subpackets, and each subpacket is 64 bits in size, including 8 bits of BCH ECC parity data, allowing for each packet to carry up to 224 bits of audio data. Each data island period can contain up to 18 packets. Seven of the 15 packet types described in the HDMI 1.3a specifications deal with audio data, while the other 8 types deal with auxiliary data. Among these are the general control packet and the gamut metadata packet. The general control packet carries information on AVMUTE (which mutes the audio during changes that may cause audio noise) and color depth (which sends the bit depth of the current video stream and is required for deep color). The gamut metadata packet carries information on the color space being used for the current video stream and is required for xvYCC.

#### Consumer Electronics Control (CEC)
Consumer Electronics Control (CEC) is an HDMI feature designed to allow the user to command and control up to 15 CEC-enabled devices, that are connected through HDMI, by using only one of their remote controls (for example by controlling a television set, set-top box, and DVD player using only the remote control of the TV). CEC also allows for individual CEC-enabled devices to command and control each other without user intervention.

It is a one-wire bidirectional serial bus that is based on the CENELEC standard AV.link protocol to perform remote control functions. CEC wiring is mandatory, although implementation of CEC in a product is optional. It was defined in HDMI Specification 1.0 and updated in HDMI 1.2, HDMI 1.2a and HDMI 1.3a (which added timer and audio commands to the bus). USB to CEC adapters exist that allow a computer to control CEC-enabled devices.

#### HDMI Ethernet and Audio Return Channel
Introduced in HDMI 1.4, HDMI Ethernet and Audio Return Channel (HEAC) adds a high-speed bidirectional data communication link (HEC) and the ability to send audio data upstream to the source device (ARC). HEAC utilizes two lines from the connector: the previously unused Reserved pin (called HEAC+) and the Hot Plug Detect pin (called HEAC−). If only ARC transmission is required, a single mode signal using the HEAC+ line can be used, otherwise, HEC is transmitted as a differential signal over the pair of lines, and ARC as a common mode component of the pair.

#### Audio Return Channel (ARC)
ARC is an audio link meant to replace other cables between the TV and the A/V receiver or speaker system. This direction is used when the TV is the one that generates or receives the video stream instead of the other equipment. A typical case is the running of an app on a smart TV such as Netflix, but reproduction of audio is handled by the other equipment. Without ARC, the audio output from the TV must be routed by another cable, typically TOSLink or RCA, into the speaker system.

#### HDMI Ethernet Channel (HEC)
HDMI Ethernet Channel technology consolidates video, audio, and data streams into a single HDMI cable, and the HEC feature enables IP-based applications over HDMI and provides a bidirectional Ethernet communication at 100 Mbit/s. The physical layer of the Ethernet implementation uses a hybrid to simultaneously send and receive attenuated 100BASE-TX-type signals through a single twisted pair.

## Versions
### 1.0
HDMI 1.0 was released on December 9, 2002, and is a single-cable digital audio/video connector interface. The link architecture is based on DVI, using exactly the same video transmission format but sending audio and other auxiliary data during the blanking intervals of the video stream. HDMI 1.0 allows a maximum TMDS clock of 165 MHz (4.95 Gbit/s bandwidth per link), the same as DVI. It defines two connectors called Type A and Type B, with pinouts based on the Single-Link DVI-D and Dual-Link DVI-D connectors respectively, though the Type B connector was never used in any commercial products. HDMI 1.0 uses TMDS encoding for video transmission, giving it 3.96 Gbit/s of video bandwidth (1920 × 1080 or 1920 × 1200 at 60 Hz) and 8-channel LPCM/192 kHz/24-bit audio. HDMI 1.0 requires support for RGB video, with optional support for Y′CBCR 4:4:4 and 4:2:2 (mandatory if the device has support for Y′CBCR on other interfaces). Color depth of 10 bpc (30 bit/px) or 12 bpc (36 bit/px) is allowed when using 4:2:2 subsampling, but only 8 bpc (24 bit/px) color depth is permitted when using RGB or Y′CBCR 4:4:4. Only the Rec. 601 and Rec. 709 color spaces are supported. HDMI 1.0 allows only specific pre-defined video formats, including all the formats defined in EIA/CEA-861-B and some additional formats listed in the HDMI Specification itself. All HDMI sources/sinks must also be capable of sending/receiving native Single-Link DVI video and be fully compliant with the DVI Specification.

### 1.1
HDMI 1.1 was released on May 20, 2004, and added support for DVD-Audio.

### 1.2
HDMI 1.2 was released on August 8, 2005, and added the option of One Bit Audio, used on Super Audio CDs, at up to 8 channels. To make HDMI more suitable for use on PC devices, version 1.2 also removed the requirement that only explicitly supported formats be used. It added the ability for manufacturers to create vendor-specific formats, allowing any arbitrary resolution and refresh rate rather than being limited to a pre-defined list of supported formats. In addition, it added explicit support for several new formats including 720p at 100 and 120 Hz and relaxed the pixel format support requirements so that sources with only native RGB output (PC sources) would not be required to support Y′CBCR output.

HDMI 1.2a was released on December 14, 2005 and fully specifies Consumer Electronic Control (CEC) features, command sets and CEC compliance tests.

### 1.3
HDMI 1.3 was released on June 22, 2006, and increased the maximum TMDS clock to 340 MHz (10.2 Gbit/s). Like previous versions, it uses TMDS encoding, giving it a maximum video bandwidth of 8.16 Gbit/s (sufficient for 1920 × 1080 at 144 Hz or 2560 × 1440 at 75 Hz). It added support for 10 bpc, 12 bpc, and 16 bpc color depth (30, 36, and 48 bit/px), called deep color. It also added support for the xvYCC color space, in addition to the ITU-R BT.601 and BT.709 color spaces supported by previous versions, and added the ability to carry metadata defining color gamut boundaries. It also optionally allows output of Dolby TrueHD and DTS-HD Master Audio streams for external decoding by AV receivers. It incorporates automatic audio syncing (audio video sync) capability. It defined cable Categories 1 and 2, with Category 1 cable being tested up to 74.25 MHz and Category 2 being tested up to 340 MHz. It also added the new HDMI Type C "Mini" connector for portable devices.

HDMI 1.3a was released on November 10, 2006, and had cable and sink modifications for HDMI Type C, source termination recommendations, and removed undershoot and maximum rise/fall time limits. It also changed CEC capacitance limits, and CEC commands for timer control were brought back in an altered form, with audio control commands added. It also added the optional ability to stream SACD in its bitstream DST format rather than uncompressed raw DSD.

### 1.4
HDMI 1.4 was released on June 5, 2009, and first came to market after Q2 of 2009. Retaining the bandwidth of the previous version, HDMI 1.4 defined standardized timings to use for 4096 × 2160 at 24 Hz, 3840 × 2160 at 24, 25, and 30 Hz, and added explicit support for 1920 × 1080 at 120 Hz with CTA-861 timings. It also added an HDMI Ethernet Channel (HEC) that accommodates a 100 Mbit/s Ethernet connection between the two HDMI connected devices so they can share an Internet connection, introduced an audio return channel (ARC), 3D Over HDMI, a new Micro HDMI Connector, an expanded set of color spaces with the addition of sYCC601, Adobe RGB and Adobe YCC601, and an Automotive Connection System. HDMI 1.4 defined several stereoscopic 3D formats including field alternative (interlaced), frame packing (a full resolution top-bottom format), line alternative full, side-by-side half, side-by-side full, 2D + depth, and 2D + depth + graphics + graphics depth (WOWvx). HDMI 1.4 requires that 3D displays implement the frame packing 3D format at either 720p50 and 1080p24 or 720p60 and 1080p24. High Speed HDMI cables as defined in HDMI 1.3 work with all HDMI 1.4 features except for the HDMI Ethernet Channel, which requires the new High Speed HDMI Cable with Ethernet defined in HDMI 1.4.

HDMI 1.4a was released on March 4, 2010, and added two mandatory 3D formats for broadcast content, which was deferred with HDMI 1.4 pending the direction of the 3D broadcast market. HDMI 1.4a has defined mandatory 3D formats for broadcast, game, and movie content. HDMI 1.4a requires that 3D displays implement the frame packing 3D format at either 720p50 and 1080p24 or 720p60 and 1080p24, side-by-side horizontal at either 1080i50 or 1080i60, and top-and-bottom at either 720p50 and 1080p24 or 720p60 and 1080p24.

HDMI 1.4b was released on October 11, 2011, containing only minor clarifications to the 1.4a document. HDMI 1.4b is the last version of the standard that HDMI LA is responsible for. All future versions of the HDMI Specification were produced by the HDMI Forum, created on October 25, 2011.

### 2.0
HDMI 2.0, referred to by some manufacturers as HDMI UHD, was released on September 4, 2013.

HDMI 2.0 increases the maximum bandwidth to 18.0 Gbit/s. HDMI 2.0 uses TMDS encoding for video transmission like previous versions, giving it a maximum video bandwidth of 14.4 Gbit/s. This enables HDMI 2.0 to carry 4K video at 60 Hz with 24 bit/px color depth. Other features of HDMI 2.0 include support for the Rec. 2020 color space, up to 32 audio channels, up to 1536 kHz audio sample frequency, dual video streams to multiple users on the same screen, up to four audio streams, 4:2:0 chroma subsampling, 25 fps 3D formats, support for the 21:9 aspect ratio, dynamic synchronization of video and audio streams, the HE-AAC and DRA audio standards, improved 3D capability, and additional CEC functions.

HDMI 2.0a was released on April 8, 2015, and added support for High Dynamic Range (HDR) video with static metadata.

HDMI 2.0b was released March 2016. HDMI 2.0b initially supported the same HDR10 standard as HDMI 2.0a as specified in the CTA-861.3 specification. In December 2016 additional support for HDR Video transport was added to HDMI 2.0b in the CTA-861-G specification, which extends the static metadata signaling to include hybrid log–gamma (HLG).

### 2.1
HDMI 2.1 was officially announced by the HDMI Forum on January 4, 2017, and was released on November 28, 2017. It adds support for higher resolutions and higher refresh rates, including 4K 120 Hz and 8K 60 Hz. HDMI 2.1 also introduces a new HDMI cable category called Ultra High Speed (referred to as 48G during development), which certifies cables at the new higher speeds that these formats require. Ultra High Speed HDMI cables are backwards compatible with older HDMI devices, and older cables are compatible with new HDMI 2.1 devices, though the full 48 Gbit/s bandwidth is only supported with the new cables.

The following features were added to the HDMI 2.1 Specification:
- Maximum supported format is 10K at 120 Hz
- Dynamic HDR for specifying HDR metadata on a scene-by-scene or even a frame-by-frame basis
    - Note: While HDMI 2.1 did standardize transport of dynamic HDR metadata over HDMI, in actuality it only formalized dynamic metadata interfaces already utilized by Dolby Vision and HDR10+ in HDMI 2.0, which is why neither Dolby Vision nor HDR10+ require HDMI 2.1 to function properly.
- Display Stream Compression (DSC) 1.2 is used for video formats higher than 8K with 4:2:0 chroma subsampling
- High Frame Rate (HFR) for 4K, 8K, and 10K, which adds support for refresh rates up to 120 Hz
- Enhanced Audio Return Channel (eARC) for object-based audio formats such as Dolby Atmos and DTS:X
- Enhanced refresh rate and latency reduction features:
    - Variable Refresh Rate (VRR) reduces or eliminates lag, stutter and frame tearing for more fluid motion in games
    - Quick Media Switching (QMS) for movies and video eliminates the delay that can result in blank screens before content begins to be displayed
    - Quick Frame Transport (QFT) reduces latency by bursting individual pictures across the HDMI link as fast as possible when the link's hardware supports more bandwidth than the minimum amount needed for the resolution and frame rate of the content. With QFT, individual pictures arrive earlier and some hardware blocks can be fully powered off for longer periods of time between pictures to reduce heat generation and extend battery life.
- Auto Low Latency Mode (ALLM) – When a display device supports the option to either optimize its pixel processing for best latency or best pixel processing, ALLM allows the current HDMI source device to automatically select, based on its better understanding of the nature of its own content, which mode the user would most likely prefer.

Video formats that require more bandwidth than 18.0 Gbit/s (4K 60 Hz 8 bpc RGB), such as 4K 60 Hz 10 bpc (HDR), 4K 120 Hz, and 8K 60 Hz, may require the new "Ultra High Speed" or "Ultra High Speed with Ethernet" cables. HDMI 2.1's other new features are supported with existing HDMI cables.

The increase in maximum bandwidth is achieved by increasing both the bitrate of the data channels and the number of channels. Previous HDMI versions use three data channels (each operating at up to 6.0 Gbit/s in HDMI 2.0, or up to 3.4 Gbit/s in HDMI 1.4), with an additional channel for the TMDS clock signal, which runs at a fraction of the data channel speed (one tenth the speed, or up to 340 MHz, for signaling rates up to 3.4 Gbit/s; one fortieth the speed, or up to 150 MHz, for signaling rates between 3.4 and 6.0 Gbit/s). HDMI 2.1 doubles the signaling rate of the data channels to 12 Gbit/s. The structure of the data has been changed to use a new packet-based format with an embedded clock signal, which allows what was formerly the TMDS clock channel to be used as a fourth data channel instead, increasing the signaling rate across that channel to 12 Gbit/s as well. These changes increase the aggregate bandwidth from 18.0 Gbit/s (3 × 6.0 Gbit/s) to 48.0 Gbit/s (4 × 12.0 Gbit/s), a 2.66× improvement in bandwidth. In addition, the data is transmitted more efficiently by using a 16b/18b encoding scheme, which uses a larger percentage of the bandwidth for data rather than DC balancing compared to the TMDS scheme used by previous versions (88.8% compared to 80%). This, in combination with the 2.66× bandwidth, raises the maximum data rate of HDMI 2.1 from 14.4 Gbit/s to 42.6 Gbit/s. Subtracting overhead for FEC, the usable data rate is approximately 42.0 Gbit/s, around 2.92× the data rate of HDMI 2.0.

The 48 Gbit/s bandwidth provided by HDMI 2.1 is enough for 8K resolution at approximately 50 Hz, with 8 bpc RGB or Y′CBCR 4:4:4 color. To achieve even higher formats, HDMI 2.1 can use Display Stream Compression with a compression ratio of up to 3∶1. Using DSC, formats up to 8K (7680 × 4320) 120 Hz or 10K (10240 × 4320) 100 Hz at 8 bpc RGB/4:4:4 are possible. Using Y′CBCR with 4:2:2 or 4:2:0 chroma subsampling in combination with DSC can allow for even higher formats.

HDMI 2.1a was released on February 15, 2022, and added support for Source-Based Tone Mapping (SBTM).

### Feature support
The features defined in the HDMI Specification that an HDMI device may implement are listed below. For historical interest, the version of the HDMI Specification in which the feature was first added is also listed. All features of the HDMI Specification are optional; HDMI devices may implement any combination of these features.

Although the "HDMI version numbers" are commonly misused as a way of indicating that a device supports certain features, this notation has no official meaning and is considered improper by HDMI Licensing. There is no officially-defined correlation between features supported by a device and any claimed "version numbers", as version numbers refer to historical editions of the HDMI Specification document, not to particular classes of HDMI devices. Manufacturers are forbidden from describing their devices using HDMI version numbers, and are required to identify support for features by listing explicit support for them, but the HDMI forum has received criticism for lack of enforcement of these policies.

- Full HD Blu-ray Disc and HD DVD video (version 1.0)
- Consumer Electronic Control (CEC) (version 1.0)
- DVD-Audio (version 1.1)
- Super Audio CD (DSD) (version 1.2)
- Auto Lip-Sync Correction (version 1.3)
- Dolby TrueHD / DTS-HD Master Audio bitstream capable (version 1.3)
- Updated list of CEC commands (version 1.3a)
- 3D video (version 1.4)
- Ethernet channel (100 Mbit/s) (version 1.4)
- Audio return channel (ARC) (version 1.4)
- 4 audio streams (version 2.0)
- Dual View (version 2.0)
- Perceptual quantizer HDR EOTF (SMPTE ST 2084) (version 2.0a)
- Hybrid log–gamma (HLG) HDR EOTF (version 2.0a)
- Static HDR metadata (SMPTE ST 2086) (version 2.0a)
- Dynamic HDR metadata (SMPTE ST 2094) (version 2.0b)
- Enhanced audio return channel (eARC) (version 2.1)
- Variable Refresh Rate (VRR) (version 2.1)
- Quick Media Switching (QMS) (version 2.1)
- Quick Frame Transport (QFT) (version 2.1)
- Auto Low Latency Mode (ALLM) (version 2.1)
- Display Stream Compression (DSC) (version 2.1)
- Source-Based Tone Mapping (SBTM) (version 2.1a)
    - Even for a compressed audio codec that a given HDMI device cannot transport, the source device may be able to decode the audio codec and transmit the audio as uncompressed LPCM.
    - CEC has been in the HDMI specification since version 1.0, but only began to see implementation in consumer electronics products in 2008
    - Even for a compressed audio codec that a given HDMI version cannot transport, the source device may be able to decode the audio codec and transmit the audio as uncompressed LPCM.
    - Large number of additions and clarifications for CEC commands. One addition is CEC command, allowing for volume control of an AV receiver.