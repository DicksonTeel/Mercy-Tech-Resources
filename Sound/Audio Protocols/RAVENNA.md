RAVENNA is a solution for real-time distribution of audio and other media content in IP-based network environments. Utilising standardised network protocols and technologies, RAVENNA can operate in existing network infrastructures and is inherently fully AES67 and SMPTE ST 2110-compliant.

---

In RAVENNA, synchronisation across all nodes is achieved through IEEE1588-2008 (also referred to as Precision Time Protocol or PTPv2), another standard protocol which can be operated on IP. PTPv2 provides means for synchronising local clocks to a precision in the lower nanoseconds range with reference to a related master clock – provided that all participating switches natively support PTPv2. But even without native PTP support, the achievable precision – while varying depending on size and bandwidth utilisation of the network – will be more than sufficient to reach sample accurate synchronisation across all nodes. Sample-accurate synchronisation can even be reached across WAN connections, when local master clocks are synchronised to GPS as a common time domain reference.

---

RTP – the real-time transport protocol, as defined by the IETF is widely used and supported by numerous applications and comes with a large number of standardised payload formats. For RAVENNA, specifically RTP/AVP over UDP together with RTCP (the real-time transport control protocol) according to RFC 3550 is used. This provides the possibility to transport any RAVENNA stream across IP-based WAN connections. Basic payload formats for audio are 16 and 24-bit @48 kHz with any desired number of channels. This would allow any standard media player to potentially link to a RAVENNA stream and monitor its content – even without knowledge or support of any of the other RAVENNA-specific features or methods.

Of course, the payload format is not restricted to those basic formats as with RTP a huge variety of different payload formats for audio and video is already defined; it is even supported both in unicast and multicast mode on a per-stream basis providing the highest flexibility to match the distinct requirements of different applications. Unicast is preferred in situations where a certain stream needs to be transported to a single destination only or where the network infrastructure or application prohibits the use of multicast (e.g. across most WAN connections). On the other hand, multicast allows resource-efficient usage of network links and faster switching between available streams in situations, where a certain stream will be accessed at different locations.

---

As different services can co-exist with RAVENNA on the same network, it has to be ensured that the traffic related to RAVENNA will be expedited with priority across the network.

For IP-based traffic, several QoS schemes have been defined as standard over time. Today, DiffServ has largely supplanted other Layer 3 QoS mechanisms (such as IntServ) as the primary protocol to provide different levels of service and is widely supported by most modern managed switches. DiffServ operates on the principle of traffic classification, where each data packet is placed into a limited number of traffic classes, rather than differentiating network traffic based on the requirements of an individual stream. Each traffic class can be managed differently, ensuring preferential treatment for higher-priority traffic on the network.

Even within RAVENNA there are different priorities assigned to different classes of traffic: while traffic related to synchronisation receives highest priority, immediately followed by any real-time media traffic, control and configuration traffic will be on a lower priority level. Any non-RAVENNA traffic would receive the lowest (standard) priority and will be treated as best-effort traffic.

In order to participate in an IP-based network communication, a device must obtain a unique IP address. Then, in order to be recognized by other RAVENNA nodes, a device must announce its existence and advertise information about available services (e.g. IP address and host name, supported protocols, access information, information about available streams etc.). Service advertisement & discovery is based on the DNS-SD protocol. In order to support a wide range of application environments, RAVENNA supports two different methods for device configuration and service advertisement & discovery: in managed networks usually DHCP and DNS services are operated under management and control of a network administrator. In small networks, where usually no DHCP / DNS server is present, the zeroconf mechanism – a fully automatic, self-configuring method – will be used for auto-IP assignment and service advertisement & discovery.

---

RAVENNA offers a highly flexible latency scheme, ranging from very low latency numbers in the sub-milliseconds area up to latency numbers large enough to suit the constraints of a WAN infrastructure. Unlike in other solutions, RAVENNA does not force the latency to system-wide defaults. In fact, the latency can be set for any stream individually and depends on a number of factors:

Network infrastructure – since RAVENNA is based on IP, virtually any network infrastructure supporting IP transport can be used. Thus, transport speed and latency numbers scale directly with the performance parameters of the underlying network infrastructure. Although Fast Ethernet is supported, the use of Gigabit Ethernet (at least for the backbone links) is recommended. As faster network technologies become available, RAVENNA can gain direct advantage from them.

Packetization factor – as samples are grouped into packets before they enter the network, the number of samples per packet directly influences the latency, where fewer samples per packet results in a lower latency. RAVENNA allows packets with just one sample per channel; however, this usually results in higher bandwidth utilisation (due to framing overhead) at the expense of stream count.

Network jitter – although packets containing the payload data are generated and inserted into the network at a relatively stable and isochronic rate, they usually tend to arrive intermittently at their destination due to the influence of competing traffic on their way through the network. This is compensated for by a jitter buffer on the receiver side, which must be large enough to account for the maximum expectable delay variation. In order to minimize the negative influence of interfering traffic, RAVENNA supports the use of IP-based QoS schemes. The use of DiffServ (DSCP) is highly recommended as it is supported by most managed switches and requires only very moderate administrative interaction as most switches already come with a pre-configured setup for DSCP support.

---

A fundamental part of the RAVENNA standard is the almost limitless configuration options that allow you to fine tune network audio streams between devices to best suit the application and hardware involved. In order to assist with the operation and choice of these configuration options the concept of profiles has been designed. All RAVENNA devices must have the ability to connect using a ‘generic’ profile, which has been defined as follows:

Channels – 1..8
Bit depth (word length) – 16 and 24
Sample frequency – 48kHz
Frames per packet – 64 (1.33 ms packet time)

Other defined profiles include:
- Generic profile
- High performance profile
- Ultra-low latency profile
- AES67 profile
- ST2110 profile

It is also possible to define your own profile (or tweak an existing one) to aid in the configuration of your particular project or application. Ease of use of different profiles will be aided in the future by the development and implementation of the Ember+ protocol. Configuration of a product's RAVENNA I/O streams is done using an embedded web page served up by the device in question. Once you have defined your configuration the stream is then available on the network and other devices can select and use it.