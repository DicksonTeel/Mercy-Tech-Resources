## Summary
DisplayPort (DP) is a digital display interface developed by a consortium of PC and chip manufacturers and standardized by the Video Electronics Standards Association (VESA). It is primarily used to connect a video source to a display device such as a computer monitor. It can also carry audio, USB, and other forms of data.

DisplayPort was designed to replace VGA, FPD-Link, and Digital Visual Interface (DVI). It is backward compatible with other interfaces, such as HDMI and DVI, through the use of either active or passive adapters.

It is the first display interface to rely on packetized data transmission, a form of digital communication found in technologies such as Ethernet, USB, and PCI Express. It permits the use of internal and external display connections. Unlike legacy standards that transmit a clock signal with each output, its protocol is based on small data packets known as micro packets, which can embed the clock signal in the data stream, allowing higher resolution using fewer pins. The use of data packets also makes it extensible, meaning more features can be added over time without significant changes to the physical interface.

DisplayPort can be used to transmit audio and video simultaneously, although each can be transmitted without the other. The video signal path can range from six to sixteen bits per color channel, and the audio path can have up to eight channels of 24-bit, 192 kHz uncompressed PCM audio. A bidirectional, half-duplex auxiliary channel carries device management and device control data for the Main Link, such as VESA EDID, MCCS, and DPMS standards. The interface is also capable of carrying bidirectional USB signals.

The interface uses an LVDS signal protocol that is not compatible with DVI or HDMI. However, dual-mode DisplayPort ports are designed to transmit a single-link DVI or HDMI protocol (TMDS) across the interface through the use of an external passive adapter, enabling compatibility mode and converting the signal from 3.3 to 5 volts. For analog VGA/YPbPr and dual-link DVI, a powered active adapter is required for compatibility and does not rely on dual mode. Active VGA adapters are powered directly by the DisplayPort connector, while active dual-link DVI adapters typically rely on an external power source such as USB.

## Versions
### 1.0 to 1.1
The first version, 1.0, was approved by VESA on 3 May 2006. Version 1.1 was ratified on 2 April 2007, and version 1.1a was ratified on 11 January 2008.

DisplayPort 1.0–1.1a allow a maximum bandwidth of 10.8 Gbit/s (8.64 Gbit/s data rate) over a standard 4-lane main link. DisplayPort cables up to 2 meters in length are required to support the full 10.8 Gbit/s bandwidth. DisplayPort 1.1 allows devices to implement alternative link layers such as fiber optic, allowing a much longer reach between source and display without signal degradation, although alternative implementations are not standardized. It also includes HDCP in addition to DisplayPort Content Protection (DPCP). The DisplayPort 1.1a standard can be downloaded for free from the VESA website.

### 1.2
DisplayPort version 1.2 was introduced on 7 January 2010. The most significant improvement of this version is the doubling of the data rate to 17.28 Gbit/s in High Bit Rate 2 (HBR2) mode, which allows increased resolutions, higher refresh rates, and greater color depth, such as 3840 × 2160 at 60 Hz 10 bpc RGB. Other improvements include multiple independent video streams (daisy-chain connection with multiple monitors) called Multi-Stream Transport, facilities for stereoscopic 3D, increased AUX channel bandwidth (from 1 Mbit/s to 720 Mbit/s), more color spaces including xvYCC, scRGB, and Adobe RGB 1998, and Global Time Code (GTC) for sub 1 μs audio/video synchronisation. Also Apple Inc.'s Mini DisplayPort connector, which is much smaller and designed for laptop computers and other small devices, is compatible with the new standard.

### 1.2a
DisplayPort version 1.2a was released in January 2013 and may optionally include VESA's Adaptive Sync. AMD's FreeSync uses the DisplayPort Adaptive-Sync feature for operation. FreeSync was first demonstrated at CES 2014 on a Toshiba Satellite laptop by making use of the Panel-Self-Refresh (PSR) feature from the Embedded DisplayPort standard, and after a proposal from AMD, VESA later adapted the Panel-Self-Refresh feature for use in standalone displays and added it as an optional feature of the main DisplayPort standard under the name "Adaptive-Sync" in version 1.2a. As it is an optional feature, support for Adaptive-Sync is not required for a display to be DisplayPort 1.2a-compliant.

### 1.3
DisplayPort version 1.3 was approved on 15 September 2014. This standard increases overall transmission bandwidth to 32.4 Gbit/s with the new HBR3 mode featuring 8.1 Gbit/s per lane (up from 5.4 Gbit/s with HBR2 in version 1.2), for a total data throughput of 25.92 Gbit/s after factoring in 8b/10b encoding overhead. This bandwidth is enough for a 4K UHD display (3840 × 2160) at 120 Hz with 24 bit/px RGB color, a 5K display (5120 × 2880) at 60 Hz with 30 bit/px RGB color, or an 8K UHD display (7680 × 4320) at 30 Hz with 24 bit/px RGB color. Using Multi-Stream Transport (MST), a DisplayPort port can drive two 4K UHD (3840 × 2160) displays at 60 Hz, or up to four WQXGA (2560 × 1600) displays at 60 Hz with 24 bit/px RGB color. The new standard includes mandatory Dual-mode for DVI and HDMI adapters, implementing the HDMI 2.0 standard and HDCP 2.2 content protection. The Thunderbolt 3 connection standard was originally to include DisplayPort 1.3 capability, but the final release ended up with only version 1.2. The VESA's Adaptive Sync feature in DisplayPort version 1.3 remains an optional part of the specification.

### 1.4
DisplayPort version 1.4 was published 1 March 2016. No new transmission modes are defined, so HBR3 (32.4 Gbit/s) as introduced in version 1.3 still remains as the highest available mode. DisplayPort 1.4 adds support for Display Stream Compression 1.2 (DSC), Forward Error Correction, HDR10 metadata defined in CTA-861.3, including static and dynamic metadata and the Rec. 2020 color space, for HDMI interoperability, and extends the maximum number of inline audio channels to 32.

DSC is a compression algorithm that reduces the size of the data stream by up to a 3:1 ratio. Although not mathematically lossless, DSC meets the ISO 29170 standard for "visually lossless" compression in most images, which cannot be distinguished from uncompressed video. Using DSC with HBR3 transmission rates, DisplayPort 1.4 can support 8K UHD (7680 × 4320) at 60 Hz or 4K UHD (3840 × 2160) at 120 Hz with 30 bit/px RGB color and HDR. 4K at 60 Hz 30 bit/px RGB/HDR can be achieved without the need for DSC. On displays which do not support DSC, the maximum limits are unchanged from DisplayPort 1.3 (4K 120 Hz, 5K 60 Hz, 8K 30 Hz).

### 1.4a
DisplayPort version 1.4a was published in April 2018. VESA made no official press release for this version. It updated DisplayPort's DSC implementation from DSC 1.2 to 1.2a.

### 2.0
On 26 June 2019, VESA formally released the DisplayPort 2.0 standard. VESA stated that version 2.0 is the first major update to the DisplayPort standard since March 2016, and provides up to a ≈3× improvement in data rate (from 25.92 to 77.37 Gbit/s) compared to the previous version of DisplayPort (1.4a), as well as new capabilities to address the future performance requirements of traditional displays. These include beyond 8K resolutions, higher refresh rates and high dynamic range (HDR) support at higher resolutions, improved support for multiple display configurations, as well as improved user experience with augmented/virtual reality (AR/VR) displays, including support for 4K-and-beyond VR resolutions.

Products incorporating DisplayPort 2.0 are not projected by VESA to appear on the market until later in 2021.

According to a roadmap published by VESA in September 2016, a new version of DisplayPort was intended to be launched in "early 2017". It would have improved the link rate from 8.1 to 10.0 Gbit/s, a 23% increase. This would have increased the total bandwidth from 32.4 Gbit/s to 40.0 Gbit/s. However, no new version was released in 2017, likely delayed to make further improvements after the HDMI Forum announced in January 2017 that their next standard (HDMI 2.1) would offer up to 48 Gbit/s of bandwidth. According to a press release on 3 January 2018, "VESA is also currently engaged with its members in the development of the next DisplayPort standard generation, with plans to increase the data rate enabled by DisplayPort by two-fold and beyond. VESA plans to publish this update within the next 18 months." At CES 2019, VESA announced that the new version would support 8K @ 60 Hz without compression and was expected to be released in the first half of 2019.

### DP 2.0 configuration examples
With the increased bandwidth enabled by DisplayPort 2.0, VESA offers a high degree of versatility and configurations for higher display resolutions and refresh rates. In addition to the above-mentioned 8K resolution at 60 Hz with HDR support, UHBR20 through USB-C as DisplayPort Alt Mode enables a variety of high-performance configurations:

**Single display resolutions**
- One 16K (15360 × 8640) display @ 60 Hz with 10 bpc (30 bit/px, HDR) RGB/Y′CBCR 4:4:4 color (with DSC)
- One 10K (10240 × 4320) display @ 60 Hz and 8 bpc (24 bit/px, SDR) RGB/Y′CBCR 4:4:4 color (uncompressed)

**Dual display resolutions**
- Two 8K (7680 × 4320) displays @ 120 Hz and 10 bpc (30 bit/px, HDR) RGB/Y′CBCR 4:4:4 color (with DSC)
- Two 4K (3840 × 2160) displays @ 144 Hz and 8 bpc (24 bit/px, SDR) RGB/Y′CBCR 4:4:4 color (uncompressed)

**Triple display resolutions**
- Three 10K (10240 × 4320) displays @ 60 Hz and 10 bpc (30 bit/px, HDR) RGB/Y′CBCR 4:4:4 color (with DSC)
- Three 4K (3840 × 2160) displays @ 90 Hz and 10 bpc (30 bit/px, HDR) RGB/Y′CBCR 4:4:4 color (uncompressed)

When using only two lanes on the USB-C connector via DP Alt Mode to allow for simultaneous SuperSpeed USB data and video, DP 2.0 can enable such configurations as:
- Three 4K (3840 × 2160) displays @ 144 Hz and 10 bpc (30 bit/px, HDR) RGB/Y′CBCR 4:4:4 color (with DSC)
- Two 4K × 4K (4096 × 4096) displays (for AR/VR headsets) @ 120 Hz and 10 bpc (30 bit/px, HDR) RGB/Y′CBCR 4:4:4 color (with DSC)
- Three QHD (2560 × 1440) @ 120 Hz and 8 bpc (24 bit/px, SDR) RGB/Y′CBCR 4:4:4 color (uncompressed)
- One 8K (7680 × 4320) display @ 30 Hz and 10 bpc (30 bit/px, HDR) RGB/Y′CBCR 4:4:4 color (uncompressed)

### 2.1
VESA announced version 2.1 of the DisplayPort standard on 17 October 2022. This version incorporates the new DP40 and DP80 cable certifications, which test DisplayPort cables for proper operation at the UHBR10 (40 Gbit/s) and UHBR20 (80 Gbit/s) speeds introduced in version 2.0. Additionally, it revises some of the electrical requirements for DisplayPort devices in order to improve integration with USB4. In VESA's words:

*DisplayPort 2.1 has tightened its alignment with the USB Type-C specification as well as the USB4 PHY specification to facilitate a common PHY servicing both DisplayPort and USB4. In addition, DisplayPort 2.1 has added a new DisplayPort bandwidth management feature to enable DisplayPort tunneling to coexist with other I/O data traffic more efficiently over the USB4 link.*

## Specifications
### Main link
The DisplayPort main link is used for transmission of video and audio. The main link consists of a number of unidirectional serial data channels which operate concurrently, called lanes. A standard DisplayPort connection has 4 lanes, though some applications of DisplayPort implement more, such as the Thunderbolt 3 interface which implements up to 8 lanes of DisplayPort.

In a standard DisplayPort connection, each lane has a dedicated set of twisted-pair wires, and transmits data across it using differential signaling. This is a self-clocking system, so no dedicated clock signal channel is necessary. Unlike DVI and HDMI, which vary their transmission speed to the exact rate required for the specific video format, DisplayPort only operates at a few specific speeds; any excess bits in the transmission are filled with "stuffing symbols".

In DisplayPort versions 1.0–1.4a, the data is encoded using ANSI 8b/10b encoding prior to transmission. With this scheme, only 8 out of every 10 transmitted bits represent data; the extra bits are used for DC balancing (ensuring a roughly equal number of 1s and 0s). As a result, the rate at which data can be transmitted is only 80% of the physical bitrate. The transmission speeds are also sometimes expressed in terms of the "Link Symbol Rate", which is the rate at which these 8b/10b-encoded symbols are transmitted (i.e. the rate at which groups of 10 bits are transmitted, 8 of which represent data).

The following transmission modes are defined in version 1.0–1.4a:
- RBR (Reduced Bit Rate): 1.62 Gbit/s bandwidth per lane (162 MHz link symbol rate)
- HBR (High Bit Rate): 2.70 Gbit/s bandwidth per lane (270 MHz link symbol rate)
- HBR2 (High Bit Rate 2): 5.40 Gbit/s bandwidth per lane (540 MHz link symbol rate), introduced in DP 1.2
- HBR3 (High Bit Rate 3): 8.10 Gbit/s bandwidth per lane (810 MHz link symbol rate), introduced in DP 1.3
- DisplayPort 2.0 uses 128b/132b encoding; each group of 132 transmitted bits represents 128 bits of data. This scheme has an efficiency of 96.96%. In addition, a small amount of overhead is added for the link layer control packet and other miscellaneous operations, resulting in an overall efficiency of ≈96.7%.

The following transmission modes are added in DP 2.0:
- UHBR 10 (Ultra High Bit Rate 10): 10.0 Gbit/s bandwidth per lane
- UHBR 13.5 (Ultra High Bit Rate 13.5): 13.5 Gbit/s bandwidth per lane
- UHBR 20 (Ultra High Bit Rate 20): 20.0 Gbit/s bandwidth per lane

The total bandwidth of the main link in a standard 4-lane connection is the aggregate of all lanes:
- RBR: 4 × 1.62 Gbit/s = 6.48 Gbit/s bandwidth (data rate of 5.184 Gbit/s or 648 MB/s with 8b/10b encoding)
- HBR: 4 × 2.70 Gbit/s = 10.80 Gbit/s bandwidth (data rate of 8.64 Gbit/s or 1.08 GB/s)
- HBR2: 4 × 5.40 Gbit/s = 21.60 Gbit/s bandwidth (data rate of 17.28 Gbit/s or 2.16 GB/s)
- HBR3: 4 × 8.10 Gbit/s = 32.40 Gbit/s bandwidth (data rate of 25.92 Gbit/s or 3.24 GB/s)
- UHBR 10: 4 × 10.0 Gbit/s = 40.00 Gbit/s bandwidth (data rate of 38.69 Gbit/s or 4.84 GB/s with 128b/132b encoding and FEC)
- UHBR 13.5: 4 × 13.5 Gbit/s = 54.00 Gbit/s bandwidth (data rate of 52.22 Gbit/s or 6.52 GB/s)
- UHBR 20: 4 × 20.0 Gbit/s = 80.00 Gbit/s bandwidth (data rate of 77.37 Gbit/s or 9.69 GB/s)
The transmission mode used by the DisplayPort main link is negotiated by the source and sink device when a connection is made, through a process called Link Training. This process determines the maximum possible speed of the connection. If the quality of the DisplayPort cable is insufficient to reliably handle HBR2 speeds for example, the DisplayPort devices will detect this and switch down to a lower mode to maintain a stable connection. The link can be re-negotiated at any time if a loss of synchronization is detected. 

Audio data is transmitted across the main link during the video blanking intervals (short pauses between each line and frame of video data).

### Auxiliary channel
The DisplayPort AUX channel is a half-duplex (bidirectional) data channel used for miscellaneous additional data beyond video and audio, such as EDID (I2C) or CEC commands. This bidirectional data channel is required, since the video lane signals are unidirectional from source to display. AUX signals are transmitted across a dedicated set of twisted-pair wires. DisplayPort 1.0 specified Manchester encoding with a 2 Mbaud signal rate (1 Mbit/s data rate). Version 1.2 of the DisplayPort standard introduced a second transmission mode called FAUX (Fast AUX), which operated at 720 Mbaud with 8b/10b encoding (576 Mbit/s data rate), but it was deprecated in version 1.3.

## Cables & Connectors
### Cables
All DisplayPort cables are compatible with all DisplayPort devices, regardless of the version of each device or the cable certification level. Additionally, all features of DisplayPort will function across any DisplayPort cable.

DisplayPort does not have multiple cable designs; all DP cables have the same basic layout and wiring, and will support any feature including audio, daisy-chaining, G-Sync/FreeSync, HDR, and DSC. Where DisplayPort cables differ is in their transmission speed support.

DisplayPort specifies seven different transmission modes (RBR, HBR, HBR2, HBR3, UHBR 10, UHBR 13.5, and UHBR 20) which support progressively higher bandwidths. Not all DisplayPort cables are capable of all seven transmission modes. VESA offers certifications for various levels of bandwidth. These certifications are optional, and not all DisplayPort cables are certified by VESA. Cables with limited transmission speed are still compatible with all DisplayPort devices, but may place limits on the maximum resolution or refresh rate available.

DisplayPort cables are not classified by "version" like you would find with protocols like HDMI. Although cables are commonly labeled with version numbers, with HBR2 cables advertised as "DisplayPort 1.2 cables" for example, this notation is not permitted by VESA. The use of version numbers with cables can falsely imply that a DisplayPort 1.4 display requires a "DisplayPort 1.4 cable", or that features introduced in version 1.4 such as HDR or DSC will not function with older "DP 1.2 cables". DisplayPort cables are classified only by their bandwidth certification level (RBR, HBR, HBR2, HBR3, etc.), if they have been certified at all. Not all DisplayPort cables are capable of functioning at the highest levels of bandwidth. Cables may be submitted to VESA for an optional certification at various bandwidth levels. VESA offers four levels of cable certification: Standard, DP8K, DP40, and DP80. These certify DisplayPort cables for proper operation at the following speeds:

| DisplayPort cable certifications |  |  |
| ----------------- | --------------------- | ------------------------------------ |
| **Transmission mode** | **Transmission bit rate**  | **Minimum required cable certification** |
| RBR (Reduced Bit Rate)              |	6.48 Gbit/s  |	Standard VESA-certified DisplayPort cable |
| HBR (High Bit Rate)                 |	10.80 Gbit/s |  Standard VESA-certified DisplayPort cable |
| HBR2 (High Bit Rate 2)              |	21.60 Gbit/s |  Standard VESA-certified DisplayPort cable |
| HBR3 (High Bit Rate 3)              |	32.40 Gbit/s |	DP8K DisplayPort cable |
| UHBR10 (Ultra High Bit Rate 10)     |	40.00 Gbit/s |	DP40 cable |
| UHBR13.5 (Ultra High Bit Rate 13.5) |	54.00 Gbit/s |	DP80 cable |
| UHBR20 (Ultra High Bit Rate 20)     |	80.00 Gbit/s |  DP80 cable |

#### Cable length
The DisplayPort standard does not specify any maximum length for cables, though the DisplayPort 1.2 standard does set a minimum requirement that all cables up to 2 meters in length must support HBR2 speeds (21.6 Gbit/s), and all cables of any length must support RBR speeds (6.48 Gbit/s). Cables longer than 2 meters may or may not support HBR/HBR2 speeds, and cables of any length may or may not support HBR3 speeds or above.

### Connectors
DisplayPort cables and ports may have either a "full-size" connector or a "mini" connector. These connectors differ only in physical shape—the capabilities of DisplayPort are the same regardless of which connector is used. Using a Mini DisplayPort connector does not affect performance or feature support of the connection.

#### Full-size DisplayPort connector
The standard DisplayPort connector (now referred to as a "full-size" connector to distinguish it from the mini connector) was the sole connector type introduced in DisplayPort 1.0. It is a 20-pin single-orientation connector with a friction lock and an optional mechanical latch. The standard DisplayPort receptacle has dimensions of 16.10 mm (width) × 4.76 mm (height) × 8.88 mm (depth).

The standard DisplayPort connector pin allocation is as follows:
- 12 pins for the main link – the main link consists of four shielded twisted pairs. Each pair requires 3 pins; one for each of the two wires, and a third for the shield. (pins 1–12)
- 2 additional ground pins – (pins 13 and 14)
- 3 pins for the auxiliary channel – the auxiliary channel uses another 3-pin shielded twisted pair (pins 15–17)
- 1 pin for HPD – hot-plug detection (pin 18)
- 2 pins for power – 3.3 V power and return line (pins 19 and 20)

#### Mini DisplayPort connector
The Mini DisplayPort connector was developed by Apple for use in their computer products. It was first announced in October 2008 for use in the new MacBooks and Cinema Display. In 2009, VESA adopted it as an official standard, and in 2010 the specification was merged into the main DisplayPort standard with the release of DisplayPort 1.2.

The Mini DisplayPort (mDP) connector is a 20-pin single-orientation connector with a friction lock. Unlike the full-size connector, it does not have an option for a mechanical latch. The mDP receptacle has dimensions of 7.50 mm (width) × 4.60 mm (height) × 4.99 mm (depth). The mDP pin assignments are the same as the full-size DisplayPort connector.

### Features
#### DisplayPort Dual-Mode (DP++)
Also called Dual-Mode DisplayPort, is a standard which allows DisplayPort sources to use simple passive adapters to connect to HDMI or DVI displays. Dual-mode is an optional feature, so not all DisplayPort sources necessarily support DVI/HDMI passive adapters, though in practice nearly all devices do. Officially, the "DP++" logo should be used to indicate a DP port that supports dual-mode, but most modern devices do not use the logo. Devices which implement dual-mode will detect that a DVI or HDMI adapter is attached, and send DVI/HDMI TMDS signals instead of DisplayPort signals.

The original DisplayPort Dual-Mode standard (version 1.0), used in DisplayPort 1.1 devices, only supported TMDS clock speeds of up to 165 MHz (4.95 Gbit/s bandwidth). This is equivalent to HDMI 1.2, and is sufficient for up to 1920 × 1200 at 60 Hz.

In 2013, VESA released the Dual-Mode 1.1 standard, which added support for up to a 300 MHz TMDS clock (9.00 Gbit/s bandwidth), and is used in newer DisplayPort 1.2 devices. This is slightly less than the 340 MHz maximum of HDMI 1.4, and is sufficient for up to 1920 × 1080 at 120 Hz, 2560 × 1440 at 60 Hz, or 3840 × 2160 at 30 Hz. Older adapters, which were only capable of the 165 MHz speed, were retroactively termed "Type 1" adapters, with the new 300 MHz adapters being called "Type 2".

##### Dual-Mode Limitations
- Limited adapter speed – Although the pinout and digital signal values transmitted by the DP port are identical to a native DVI/HDMI source, the signals are transmitted at DisplayPort's native voltage (3.3 V) instead of the 5 V used by DVI and HDMI. As a result, dual-mode adapters must contain a level-shifter circuit which changes the voltage. The presence of this circuit places a limit on how quickly the adapter can operate, and therefore newer adapters are required for each higher speed added to the standard.
- Unidirectional – Although the dual-mode standard specifies a method for DisplayPort sources to output DVI/HDMI signals using simple passive adapters, there is no counterpart standard to give DisplayPort displays the ability to receive DVI/HDMI input signals through passive adapters. As a result, DisplayPort displays can only receive native DisplayPort signals; any DVI or HDMI input signals must be converted to the DisplayPort format with an active conversion device. DVI and HDMI sources cannot be connected to DisplayPort displays using passive adapters.
- Single-link DVI only – Since DisplayPort dual-mode operates by using the pins of the DisplayPort connector to send DVI/HDMI signals, the 20-pin DisplayPort connector can only produce a single-link DVI signal (which uses 19 pins). A dual-link DVI signal uses 25 pins, and is therefore impossible to transmit natively from a DisplayPort connector through a passive adapter. Dual-link DVI signals can only be produced by converting from native DisplayPort output signals with an active conversion device.
- Unavailable on USB-C – The DisplayPort Alternate Mode specification for sending DisplayPort signals over a USB-C cable does not include support for the dual-mode protocol. As a result, DP-to-DVI and DP-to-HDMI passive adapters do not function when chained from a USB-C to DP adapter.

#### Multi-Stream Transport (MST) 
Multi-Stream Transport is a feature first introduced in the DisplayPort 1.2 standard. It allows multiple independent displays to be driven from a single DP port on the source devices by multiplexing several video streams into a single stream and sending it to a branch device, which demultiplexes the signal into the original streams. Branch devices are commonly found in the form of an MST hub, which plugs into a single DP input port and provides multiple outputs, but it can also be implemented on a display internally to provide a DP output port for daisy-chaining, effectively embedding a 2-port MST hub inside the display. Theoretically, up to 63 displays can be supported, but the combined data rate requirements of all the displays cannot exceed the limits of a single DP port (17.28 Gbit/s for a DP 1.2 port, or 25.92 Gbit/s for a DP 1.3/1.4 port). In addition, the maximum number of links between the source and any device (i.e. the maximum length of a daisy-chain) is 7, and the maximum number of physical output ports on each branch device (such as a hub) is 7. With the release of MST, standard single-display operation has been retroactively named "SST" mode (Single-Stream Transport).

Daisy-chaining is a feature that must be specifically supported by each intermediary display; not all DisplayPort 1.2 devices support it. Daisy-chaining requires a dedicated DisplayPort output port on the display. Standard DisplayPort input ports found on most displays cannot be used as a daisy-chain output. Only the last display in the daisy-chain does not need to support the feature specifically or have a DP output port. DisplayPort 1.1 displays can also be connected to MST hubs, and can be part of a DisplayPort daisy-chain if it is the last display in the chain.

The host system's software also needs to support MST for hubs or daisy-chains to work. While Microsoft Windows environments have full support for it, Apple operating systems currently do not support MST hubs or DisplayPort daisy-chaining as of macOS 10.15 ("Catalina"). DisplayPort-to-DVI and DisplayPort-to-HDMI adapters/cables may or may not function from an MST output port; support for this currently depends on the specific device.

MST is supported by USB Type-C DisplayPort Alternate Mode, so standard DisplayPort daisy-chains and MST hubs do function from Type-C sources with a simple Type-C to DisplayPort adapter.

#### High dynamic range (HDR)
Main article: High-dynamic-range television
Support for HDR video was introduced in DisplayPort 1.4. It implements the CTA 861.3 standard for transport of static HDR metadata in EDID.

#### Content protection 
DisplayPort 1.0 includes optional DPCP (DisplayPort Content Protection) from Philips, which uses 128-bit AES encryption. It also features full authentication and session key establishment. Each encryption session is independent, and it has an independent revocation system. This portion of the standard is licensed separately. It also adds the ability to verify the proximity of the receiver and transmitter, a technique intended to ensure users are not bypassing the content protection system to send data out to distant, unauthorized users.

DisplayPort 1.1 added optional implementation of industry-standard 56-bit HDCP (High-bandwidth Digital Content Protection) revision 1.3, which requires separate licensing from the Digital Content Protection LLC.

DisplayPort 1.3 added support for HDCP 2.2, which is also used by HDMI 2.0.

### Companion Standards
#### Mini DisplayPort
Mini DisplayPort (mDP) is a standard announced by Apple in the fourth quarter of 2008. Shortly after announcing Mini DisplayPort, Apple announced that it would license the connector technology with no fee. The following year, in early 2009, VESA announced that Mini DisplayPort would be included in the upcoming DisplayPort 1.2 specification. On 24 February 2011, Apple and Intel announced Thunderbolt, a successor to Mini DisplayPort which adds support for PCI Express data connections while maintaining backwards compatibility with Mini DisplayPort based peripherals.

#### Micro DisplayPort
Micro DisplayPort would have targeted systems that need ultra-compact connectors, such as phones, tablets and ultra-portable notebook computers. This standard would have been physically smaller than the currently available Mini DisplayPort connectors. The standard was expected to be released by Q2 2014.

#### DDM
Direct Drive Monitor (DDM) 1.0 standard was approved in December 2008. It allows for controller-less monitors where the display panel is directly driven by the DisplayPort signal, although the available resolutions and color depth are limited to two-lane operation.

#### Display Stream Compression
Display Stream Compression (DSC) is a VESA-developed video compression algorithm designed to enable increased display resolutions and frame rates over existing physical interfaces, and make devices smaller and lighter, with longer battery life.

#### eDP
Embedded DisplayPort (eDP) is a display panel interface standard for portable and embedded devices. It defines the signaling interface between graphics cards and integrated displays. The various revisions of eDP are based on existing DisplayPort standards. However, version numbers between the two standards are not interchangeable. For instance, eDP version 1.4 is based on DisplayPort 1.2, while eDP version 1.4a is based on DisplayPort 1.3. In practice, embedded DisplayPort has displaced LVDS as the predominant panel interface in modern laptops and modern smartphones.

eDP 1.0 was adopted in December 2008. It included advanced power-saving features such as seamless refresh rate switching. Version 1.1 was approved in October 2009 followed by version 1.1a in November 2009. Version 1.2 was approved in May 2010 and includes DisplayPort 1.2 HBR2 data rates, 120 Hz sequential color monitors, and a new display panel control protocol that works through the AUX channel. Version 1.3 was published in February 2011; it includes a new optional Panel Self-Refresh (PSR) feature developed to save system power and further extend battery life in portable PC systems. PSR mode allows the GPU to enter a power saving state in between frame updates by including framebuffer memory in the display panel controller. Version 1.4 was released in February 2013; it reduces power consumption through partial-frame updates in PSR mode, regional backlight control, lower interface voltages, and additional link rates; the auxiliary channel supports multi-touch panel data to accommodate different form factors. Version 1.4a was published in February 2015; the underlying DisplayPort version was updated to 1.3 in order to support HBR3 data rates, Display Stream Compression 1.1, Segmented Panel Displays, and partial updates for Panel Self-Refresh. Version 1.4b was published in October 2015; its protocol refinements and clarifications are intended to enable adoption of eDP 1.4b in devices by mid-2016. Version 1.5 was published in October 2021; adds new features and protocols, including enhanced support for Adaptive-Sync, that provide additional power savings and improved gaming and media playback performance.

#### iDP
Internal DisplayPort (iDP) 1.0 was approved in April 2010. The iDP standard defines an internal link between a digital TV system on a chip controller and the display panel's timing controller. It aims to replace currently used internal FPD-Link lanes with a DisplayPort connection. iDP features a unique physical interface and protocols, which are not directly compatible with DisplayPort and are not applicable to external connection, however they enable very high resolution and refresh rates while providing simplicity and extensibility. iDP features a non-variable 2.7 GHz clock and is nominally rated at 3.24 Gbit/s per lane, with up to sixteen lanes in a bank, resulting in a six-fold decrease in wiring requirements over FPD-Link for a 1080p24 signal; other data rates are also possible. iDP was built with simplicity in mind so doesn't have an AUX channel, content protection, or multiple streams; it does however have frame sequential and line interleaved stereo 3D.

#### PDMI
Portable Digital Media Interface (PDMI) is an interconnection between docking stations/display devices and portable media players, which includes 2-lane DisplayPort v1.1a connection. It has been ratified in February 2010 as ANSI/CEA-2017-A.

#### wDP
Wireless DisplayPort (wDP) enables the bandwidth and feature set of DisplayPort 1.2 for cable-free applications operating in the 60 GHz radio band. It was announced in November 2010 by WiGig Alliance and VESA as a cooperative effort.

#### SlimPort
SlimPort, a brand of Analogix products, complies with Mobility DisplayPort, also known as MyDP, which is an industry standard for a mobile audio/video Interface, providing connectivity from mobile devices to external displays and HDTVs. SlimPort implements the transmission of video up to 4K-UltraHD and up to eight channels of audio over the micro-USB connector to an external converter accessory or display device. SlimPort products support seamless connectivity to DisplayPort, HDMI and VGA displays. The MyDP standard was released in June 2012, and the first product to use SlimPort was Google's Nexus 4 smartphone. SlimPort is an alternative to Mobile High-Definition Link (MHL).

#### DisplayID
DisplayID is designed to replace the E-EDID standard. DisplayID features variable-length structures which encompass all existing EDID extensions as well as new extensions for 3D displays and embedded displays.

The latest version 1.3 (announced on 23 September 2013) adds enhanced support for tiled display topologies; it allows better identification of multiple video streams, and reports bezel size and locations. As of December 2013, many current 4K displays use a tiled topology, but lack a standard way to report to the video source which tile is left and which is right. These early 4K displays, for manufacturing reasons, typically use two 1920×2160 panels laminated together and are currently generally treated as multiple-monitor setups. DisplayID 1.3 also allows 8K display discovery, and has applications in stereo 3D, where multiple video streams are used.

#### DockPort
DockPort, formerly known as Lightning Bolt, is an extension to DisplayPort to include USB 3.0 data as well as power for charging portable devices from attached external displays. Originally developed by AMD and Texas Instruments, it has been announced as a VESA specification in 2014.

#### USB-C
On 22 September 2014, VESA published the DisplayPort Alternate Mode on USB Type-C Connector Standard, a specification on how to send DisplayPort signals over the newly released USB-C connector. One, two or all four of the differential pairs that USB uses for the SuperSpeed bus can be configured dynamically to be used for DisplayPort lanes. In the first two cases, the connector still can carry a full SuperSpeed signal; in the latter case, at least a non-SuperSpeed signal is available. The DisplayPort AUX channel is also supported over the two sideband signals over the same connection; furthermore, USB Power Delivery according to the newly expanded USB-PD 2.0 specification is possible at the same time. This makes the Type-C connector a strict superset of the use-cases envisioned for DockPort, SlimPort, Mini and Micro DisplayPort.

#### VirtualLink
VirtualLink is a proposal that allows the power, video, and data required to drive virtual reality headsets to be delivered over a single USB-C cable.