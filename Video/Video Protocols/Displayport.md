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