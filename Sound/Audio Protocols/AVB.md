AVB (Audio Video Bridging) is an extension to the Ethernet standard designed to provide guaranteed quality of service, which simply means that audio samples will reach their destinations on time. AVB allows you to create a single network for audio, video, and other data like control information, using an AVB-compatible switch. This enables you to mix normal network data and audio network data on the same network, making it easier to create both simple and complex networks.

AVB networking offers several features that make it ideal for audio applications:

- **Long, light cable runs**: A single lightweight CAT5e or CAT6 cable can be run up to 100 meters (328 feet). This makes it easy to have audio I/O located in different rooms (or even different venues in the same building) and run multichannel audio between them in real time.
- **Low, predictable latency**: AVB provides latency of no longer than 2 ms sending an audio stream point-to-point over up to seven “hops” (trips through switches or other devices) on a 100 Mbps network. With higher speed networks, many AVB devices support lower latencies and additional hops.
- **Scalable, with high channel counts**: AVB’s bandwidth is sufficient to carry hundreds of real-time channels using a single Ethernet cable. This offers the future possibility of expanding your system with additional devices that contain different kinds of audio I/O, multiple controllers, and other useful functions.
- **Guaranteed bandwidth**: AVB networks intelligently manage the data traffic giving priority to AVB data. This means standard network traffic, such as Internet streaming, won’t prevent your audio from being delivered reliably and on time.
- **Integrated clock signal**: In a digital audio system with multiple devices, having a master clock is critical to maintaining audio fidelity. The AVB specification defines such a clock to be accurately distributed to all devices in the system.

AVB networks behave very much like an analog audio system. Like an analog audio system, audio networks consist of sources, destinations, and intermediate processing along the way.

---

On the simplest level, AVB works by reserving a portion of the available Ethernet bandwidth for its own traffic. Because packets of AVB data are sent regularly in allocated slots within the reserved bandwidth, there are no interruptions or interference, making AVB extremely reliable.

What makes AVB ideal for audio networking is that it splits network traffic into real-time traffic and everything else. All real-time traffic is transmitted on an 8 kHz pulse. Anything that’s not real-time traffic is then transmitted around that pulse. Every 125 µs, all real-time streams send their data. Other packets are transmitted when there is no more real-time data ready to be transmitted. To make sure that there is enough bandwidth available for all prioritized real-time traffic, the Stream Reservation Protocol (SRP, IEEE 802.1Qat) is used.

Every AVB compliant switch between each talker and listener will then make sure sufficient bandwidth is available using SRP, making it a foundational building block of the AVB standard. Every switch and AVB device on the network must implement SRP and send real-time traffic at the 8 kHz pulse. If one of the devices on the network does not employ this standard, then real-time traffic could be potentially delayed, causing jitter in the output.

---

In an AVB network, every device to and from which audio is flowing must adhere to the AVB standard. These devices consist of the following types:

- **AVB Talkers**: These devices act as the source for an AVB stream, sending out audio onto the network.
- **AVB Listeners**: These devices are the destinations for the streams sent out by the Talkers.
- **AVB Switches**: This is the network hub to which every Talker and Listener must be connected. At its most basic level, an AVB Switch analyzes and prioritizes traffic on the network. It should be noted that just like there can be multiple talkers and listeners on the same AVB network, there can also be multiple AVB Switches.
- **AVB Controllers**: A controller can be a talker, a listener, or neither. These devices handle routing, clock, and other settings for AVB devices using AVDECC.
The most important rule to keep in mind when setting up an AVB network is that the talker (device sending audio) and listener (device receiving audio) must be connected to an AVB-compatible switch. All the AVB devices on the network must share a virtual clock that defines when the AVB packet should be played.

As previously mentioned, devices communicate on an AVB network as “talkers” and “listeners.” An AVB talker transmits one or more audio streams to the network. AVB listeners receive one or more of these streams from the network. It should be noted that an AVB device can be both a talker and a listener.

AVB devices stay in sync by selecting the best master PTP clock after the devices connect with one another. This ensures that every AVB device on the network will maintain precise timing, which is critical to audio quality.

The AVB switch guarantees that real-time audio data packets maintain their timing without losing information. AVB switches do this by allowing a maximum of 75% of each port to be used for AVB traffic. This prevents non-AVB data from being delayed or lost.

When an AVB network is configured, the talkers and listeners identify one another automatically.

---

SRP works with the 802.1Qav Queuing and Forwarding Protocol (Qav) to ensure that once bandwidth is reserved for an AVB stream, it is locked down from end to end. Qav schedule time-sensitive streaming information to minimize latency. Together, SRP and Qav make sure that all reserved media streams are delivered on time.

In this way, the AVB network has some intelligence as to how much non-media traffic as well as how many media packets are on the system at any given time. This means that on an AVB network, the worst case travel time is known throughout the entire system. Because of this, only a small amount of buffering is needed, lowering latency to 2 ms over seven switch hops on a 100 Mbps Ethernet network. On gigabit networks, even lower latencies can be achieved.