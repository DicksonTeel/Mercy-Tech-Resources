Network Device Interface (NDI) is a royalty-free software specification developed by NewTek to enable video-compatible products to communicate, deliver, and receive high-definition video over a computer network in a high-quality, low-latency manner that is frame accurate and suitable for switching in a live production environment.

---

NDI is designed to run over gigabit Ethernet, with the NDI codec expected to deliver 1080i HD video at VBR data rates typically around 100 Mbit/s.

By default, NDI uses the mDNS (Bonjour / Zeroconf) discovery mechanism to advertise sources on a local area network, such that NDI receiving devices can automatically discover and offer those sources, although 2 other discovery modes (NDI Access, NDI Discovery Server) allow for operations across subnets, and without mDNS. Sources are created using an arbitrarily selected TCP port from a range of ports on the NDI send host. When a source is requested, a TCP connection is established on the appropriate port with the NDI receiver connecting to the NDI sender. NDI 3.x has options to use UDP multicast or unicast with forward error correction (FEC) instead of TCP, and can load balance streams across multiple network interface controllers NICs without using link aggregation. NDI 4.0 introduces multi-TCP connections.

NDI carries video, multichannel uncompressed audio and metadata. Metadata messages can be sent in both directions allowing the sender and receiver to message one another over the connection with arbitrary metadata in XML form. This directional metadata system allows for functionality such as active tally information fed back to sources to understand that they are on-air (program / preview). NDI also allows senders to determine the number of connected receivers, so they can skip unnecessary processing and network bandwidth utilisation when there are no NDI receiver clients connected. NDI Receivers can opt to connect to various combinations of streams, to support things like audio-only or metadata-only connections where video is not required.

The NDI software development kit (SDK) is available for Windows, Linux and MacOS, and has also been ported to iOS, tvOS, Android, Raspberry Pi, and FPGA. The Standard NDI SDK is available via a royalty-free proprietary license. The NDI Advanced SDK offers OEMs direct access to and from compressed data and other features, with a commercial license.

---

NDI was publicly revealed by NewTek on 8 September 2015 and was demonstrated at the IBC broadcast exhibition in Amsterdam that week. The first device shown using NDI was the NewTek TriCaster which delivered an NDI feed from each of its SDI inputs as well as four output feeds from its vision mixer. The TriCaster could also receive up to two NDI sources from other devices (increased to 12 in later releases and up to 44 in NewTek's IP Series ).

NewTek had previously created a predecessor of NDI called AirSend to get video from external devices into their TriCaster products. AirSend had been implemented by a number of character generator (CG) vendors including Vizrt and Chyron. In order to quickly bring these products into the NDI space, NewTek created a new driver to replace the existing AirSend driver, which could be installed on these existing AirSend-compatible devices, instantly converting them to NDI-compatible devices with no change required by the original CG vendors.

Another early adopter of NDI was VMix, a Windows-based vision mixer which offers NDI inputs and outputs. A significant increase in the NDI installed base came when live streaming application XSplit added support for NDI.

Later in 2016, NewTek delivered NDI 2.0 which added features including support for service discovery across subnets. In April, Magewell announced seamless integration of their PCIe and USB capture devices, allowing access to any video source on the network. This solution created one of the most efficient broadcast video production scenarios possible with unlimited source choice and ubiquitous operating system compatibility.

On 12 July 2017 NewTek announced NDI 3.0 which added multicast, NDI|HX and other new features, introducing support for specific PTZ Cameras with H.264 chipsets and updated firmware.

In April 2019, ahead of NAB, NewTek announced the addition of Multi-TCP mode to NDI 4.0 which is reported to leverage hardware TCP acceleration present in silicon, assisting lower-spec processors with NDI transport.

In July 2021, NDI 5 has been released adding the following main features: Reliable UDP transmission, Redundant discovery server support, NDI 5 Tools (NDI Bridge, NDI Remote, NDI Audio Direct, FCP-X output)

---

NDI was designed to work on good quality gigabit local area networks using TCP and Bonjour (mDNS) technologies. In order to work across subnets that don't pass mDNS, NDI supports a mechanism known as NDI Access which allows manual entry of the IP address of machines on other subnets which may be running NDI sources.

Some NDI adopters have run the protocol across fibre connections up to 15 km, although NDI's use of the TCP protocol makes it less suitable for long-distance, high-latency connections due to factors such as bandwidth-delay product and TCP packet loss recovery. Later versions of NDI introduced different transport protocols including UDP, MultiTCP and reliable UDP (QUIC) which offer different network characteristics. NDI|HX uses a lower data rate making it easier to use in bandwidth-limited connections.

---

NDI is also used within cloud-based production systems, with its compressed video and unicast transmissions making it suitable for cloud-based services like AWS and Azure. When operating in cloud environments, the NDI Discovery service provides a solution to multicast restrictions common to cloud platforms. Starting with NDI 5, the Bridge tool allows you to connect remote locations together be it over open Internet or via a VPN. NDI Bridge allows you use NDI-HX2 at selectable bitrates and codec types (H.264 or HEVC) as the transmission format between locations (High Bandwidth NDI transmission is also possible), all other aspects of the NDI signal are preserved (metadata, alpha, tally, etc).

---

NDI can run on 32-bit or 64-bit CPU architectures, although performance is increased when using 64-bit.

NDI 4.x and earlier had limited support for ARM, generally offering encode-only support. The release of NDI 5 brings full support for encode and decode on ARM-based processors that include Neon instructions.

NDI|HX devices are typically transmit-only and based on proprietary platforms with hardware H.264 encoder chips. Examples of NDI|HX devices are PTZ cameras, and the NDI Connect Spark SDI to NDI|HX converter box. The NDI stream itself is formed at the stream consumption end via the platform-specific NDI|HX driver, presenting the same uncompressed data to the application software consuming the NDI source regardless of original HX source hardware and compression. NDI|HX2 is a purer implementation, supporting either H.264 or HEVC compression, and allows for additional NDI features.

With NDI 4.0 NewTek announced the addition of a Multi-TCP transport mode. This takes advantage of the hardware TCP acceleration in silicon which helps lower-spec processors handle heavy network load, in contrast to UDP which does not benefit from the hardware acceleration.

---

NDI supports arbitrary metadata as XML blocks, embedded in video and audio frames, as well as stand-alone metadata frames. The content of these metadata blocks form 3 families:

1. Internal metadata used by NDI invisibly. These messages are used for connectivity and some other fundamental tasks like Tally. They are typically invisible to NDI clients.
1. Defined public metadata. These messages include things like the NDI PTZ Protocol. They are defined by NewTek as part of the NDI SDK.
1. Third-party metadata schemas. These messages are implemented in the same way as defined NDI metadata but the content is based on third-party designs.