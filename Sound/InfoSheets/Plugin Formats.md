# Plugin Formats

## Audio Units (AU)
Audio Units are a system-level plug-in architecture provided by Core Audio in Apple's macOS and iOS operating systems. Audio Units are a set of application programming interface (API) services provided by the operating system to generate, process, receive, or otherwise manipulate streams of audio in near-real-time with minimal latency. It may be thought of as Apple's architectural equivalent to another popular plug-in format, Steinberg's Virtual Studio Technology (VST).

Because of the many similarities between Audio Units and VST, several commercial and free wrapping technologies are available (e.g. Symbiosis and FXpansion VST-AU Adapter). Manufacturers Celemony Software and PreSonus have also developed the Audio Random Access (ARA) extension, which works for both AU and VST, allowing greater integration between the plug-ins and DAW software.

---

## Virtual Studio Technology (VST)
Virtual Studio Technology is an audio plug-in software interface that integrates software synthesizers and effects units into digital audio workstations. VST and similar technologies use digital signal processing to simulate traditional recording studio hardware in software. Thousands of plugins exist, both commercial and freeware, and many audio applications support VST under license from its creator, Steinberg.

VST plugins generally run within a digital audio workstation (DAW), to provide additional functionality, though a few standalone plugin hosts exist that support VST. Most VST plugins are either instruments (VSTi) or effects (VSTfx), although other categories exist—for example spectrum analyzers and various meters. VST plugins usually provide a custom graphical user interface that displays controls similar to physical switches and knobs on audio hardware. Some (often older) plugins rely on the host application for their user interface.

VST instruments include software simulation emulations of hardware synthesizers and samplers. These typically emulate the look of the original equipment as well as its sonic characteristics. This lets musicians and recording engineers use virtual versions of devices that otherwise might be difficult and expensive to obtain.

VST instruments receive notes as digital information via MIDI, and output digital audio. Effect plugins receive digital audio and process it through to their outputs. (Some effect plugins also accept MIDI input—for example, MIDI sync to modulate the effect in sync with the tempo). MIDI messages can control both instrument and effect plugin parameters. Most host applications can route the audio output from one VST to the audio input of another VST (chaining). For example, the output of a VST synthesizer can be sent through a VST reverb effect.

There are three types of VST plugins:
- VST instruments generate audio. They are generally either virtual synthesizers or virtual samplers. Many recreate the look and sound of famous hardware synthesizers. Better known VST instruments include Discovery, Nexus, Sylenth1, Massive, Omnisphere, FM8, Absynth, Reaktor, Gladiator, Serum and Vanguard.
- VST effects process rather than generate audio—and perform the same functions as hardware audio processors such as reverbs and phasers. Other monitoring effects provide visual feedback of the input signal without processing the audio. Most hosts allow multiple effects to be chained. Audio monitoring devices such as spectrum analyzers and meters represent audio characteristics (frequency distribution, amplitude, etc.) visually.
- VST MIDI effects process MIDI messages (for example, transpose or arpeggiate) and route the MIDI data to other VST instruments or to hardware devices.

Steinberg released the VST interface specification and SDK in 1996. They released it at the same time as Steinberg Cubase 3.02, which included the first VST format plugins: Espacial (a reverb), Choirus (a chorus effect), Stereo Echo, and Auto-Panner.

Steinberg updated the VST interface specification to version 2.0 in 1999. One addition was the ability for plugins to receive MIDI data. This supported the introduction of Virtual Studio Technology Instrument (VSTi) format plugins. VST Instruments can act as standalone software synthesizers, samplers, or drum machines.

In 2006, the VST interface specification was updated to version 2.4. Changes included the ability to process audio with 64-bit precision.

VST 3.0 came out in 2008. Changes included:
- Audio Inputs for VST Instruments
- Multiple MIDI inputs/outputs
- Optional SKI (Steinberg Kernel Interface) integration

VST 3.5 came out in February 2011. Changes included note expression, which provides extensive articulation information in individual note events in a polyphonic arrangement. According to Steinberg, this supports performance flexibility and a more natural playing feel.

In October 2011, Celemony Software and PreSonus released Audio Random Access (ARA), an extension for audio plug-in interfaces, such as VST, allowing greater integration between audio plug-ins and DAW software.

In September, 2013, Steinberg discontinued maintenance of the VST 2 SDK. In December, Steinberg stopped distributing the SDK. The higher versions are continued.

VST 3.6.7 came out in March, 2017. It includes a preview version of VST3 for the Linux platform, the VST3 part of the SDK gets a dual license: "Proprietary Steinberg VST3" or the "Open-source GPLv3".

As VSTi virtual instrument technology was under development at Steinberg, a platform for virtual instruments using DirectX engine technology was being developed by Cakewalk, famous for its Sonar DAW. However, the format did not gain much acceptance beyond instruments bundled with SONAR. Currently, almost all virtual instruments on the market use Steinberg's VSTi format.

The VST plugin standard is the audio plugin standard created by Steinberg to allow any third-party developers to create VST plugins for use within VST host applications. VST requires separate installations for Windows, Mac OS X and Linux. A large amount of VST plugins are available for Windows only due to Apple's competing proprietary Audio Unit technology being used on OS X (Audio Units is a core part of the OS X operating system). The short history of commercial environments for Linux means few developers have targeted this platform.

VST plugins often have many controls, and therefore need a method of managing presets (sets of control settings).

Steinberg introduced two file formats for storing presets: an FXP file stores a single preset, while an FXB file stores a whole bank of presets. These formats have since been adopted by many other VST hosts, although Cubase itself switched to a new system of preset management with Cubase 4.0.

However, many VST plugins have their own method of loading and saving presets, which do not necessarily use the standard FXP/FXB formats.

---

## Avid Audio eXtension (AAX)


---

## Audio Random Access Extension (ARA)
Audio Random Access is an extension for audio plug-in interfaces allowing them to exchange a greater amount of audio information with digital audio workstation (DAW) software.

ARA was developed as a joint effort between Celemony Software and PreSonus, driven by the desire to increase the level of integration between Celemony's Melodyne plug-in and the DAWs using it. It was first published in October 2011 and released as part of PreSonus' Studio One DAW (version 2) and Melodyne (Editor, Assistant and Essential versions 1.3).

Version 2 of ARA was announced during NAMM in January 2018, introducing new features such as the simultaneous editing of multiple tracks, transfer of chord track information, and undo synchronization with the DAW. DAWs which use ARA version 2 are not automatically backwards compatible with plug-ins using version 1. The first DAWs to support ARA version 2 were Logic Pro X (version 10.4, released in January 2018) and Studio One (version 4, released in May 2018).