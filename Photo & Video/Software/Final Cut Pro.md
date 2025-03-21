Link to Apple's Final Cut Pro: [Final Cut Pro](https://www.apple.com/final-cut-pro/)

Link to Final Cut Pro Resources: [Final Cut Resources](https://www.apple.com/final-cut-pro/resources/

Final Cut Pro (often abbreviated FCP or FCPX) is a professional non-linear video-editing application initially developed by Macromedia, and, since 1998, by Apple as part of its pro apps collection. Final Cut Pro allows users to import,
edit, and process video footage, and output it to a wide variety of formats.

In the 2000s, Final Cut Pro developed a large and expanding user base, mainly video hobbyists and independent filmmakers. It also made inroads with film and television editors who have traditionally used Avid Media Composer. According
to a 2007 SCRI study, Final Cut Pro made up 49% of the United States professional editing market, with Avid at 22%. A published survey in 2008 by the American Cinema Editors Guild placed their users at 21% Final Cut Pro (and growing
from previous surveys of this group), while all others were on an Avid system of some kind. In 2011, Final Cut Pro 7 was replaced with the fully rewritten Final Cut Pro X, which initially lacked many features from previous versions,
though frequent updates have brought back many of these features. Final Cut Pro for iPad was made available on May 23, 2023.)

### Features

Final Cut Pro provides non-linear, non-destructive editing of any QuickTime-compatible video format including DV, HDV, P2 MXF (DVCProHD), XDCAM (via plug-in), 2K, 4K, 5K, and 8K film formats and can import projects directly from iMovie
for iOS and iPadOS. It supports a number of simultaneously composited video tracks (limited mainly by video form capability); unlimited audio tracks; multi-camera editing for combining video from multiple camera sources (referred to as
angles); 360º video editing support; as well as the standard ripple, roll, slip, slide, scrub, razor blade and time remapping edit functions. It comes with a range of video transitions and a range of video and audio filters such as
keying tools, mattes and vocal de-poppers and de-essers. It also has multiple color-correction tools including color wheels, sliders and curves, video scopes and a selection of generators, such as slugs, test cards, and noise. The
functionality of Final Cut Pro can be extended with plug-ins which may provide additional effects, titles, transitions, and more. Apple maintains the APIs and documentation for everyone to develop such plug-ins.

#### Interface

- Event browser: Replacing “bins” in other NLEs, the event browser is where the original media is found and can be searched and sorted by various forms of metadata. Keyword ranges, favorite and rejected ranges, and smart collections
  allow for faster sorting of a large number of clips.

- Magnetic timeline: Inventing an alternative to track-based timelines found in traditional NLEs, Final Cut's magnetic timeline uses clip connections to keep connected clips and secondary storylines in sync with clips located on the
  primary storyline. By default, clips move around each other "magnetically", filling in any gaps and avoiding clip collisions by automatically bumping clips out of the way vertically. The magnetic connections are also user-definable.

- Roles: In order to separate and organize different audio types on the magnetic timeline, editors can designate what "role" each clip plays. Introduced in version 10.0.1, Roles can be assigned to clips as an alternate way of creating
  organizational functionality. A Role (or Sub-Role) gets assigned to clips to identify what it is (for example Video, Titles, Dialogue, Effects, Music). Upon Sharing a Master File of the Project the various Roles can be split out as
  stems or in a multitrack file for broadcast delivery or other distribution needs.

- Content auto-analysis: Found in the import window and event browser is the option to analyze media for shot type and facial recognition or fix potential problems like audio loudness, audio hum, channel grouping, background noise,
  color balance, pulldown removal, and stabilization. This process generates metadata that can automatically be organized as Keywords and can be grouped into Smart Collections.

- Synchronized clips: Video and audio clips recorded on separate devices can be synched automatically by timecode, audio waveforms, and markers together as a single clip.

- Compound clips: Nested sequences from the original Final Cut Pro have been replaced by compound clips. A selection of video and audio clips can be nested into a single compound clip. This compound clip can be opened in its own
  timeline or broken apart for further editing. It can also be reused in different projects.

- Closed captions: Introduced in version 10.4.1, closed captions can be created right in the timeline or imported into the timeline from an external file.

- Multicam editing: Introduced in version 10.0.3, multiple camera angles can be synchronized automatically and combined into a multicam clip. Once in the timeline, a multicam clip can be cut up into different angles by using the angle
  viewer. A multicam clip can be opened in the angle editor where new angles can be added, synched, relabeled, and rearranged at any time.

- Auditions: Clips can be grouped together in the event browser or on the timeline as auditions. Once in the timeline, an audition allows the user to choose between different clips in their edit while the timeline ripples automatically
  in order to preview two or more different versions of a cut.

- 3D titles: Introduced in version 10.2.0, text can be extruded, textured, lit, and shaded with materials and environments in 3D. This allows users to create titles like those found in Hollywood movies directly in the application. 360
  degree video editing: Introduced in version 10.4. import and edit 360° equirectangular video in a wide range of formats and frame sizes.

- Advanced color grading

- Wide-gamut high dynamic range

#### Technical features

While inheriting the name from its predecessor, Final Cut Pro, Final Cut Pro X is a completely re-written application. As a native 64-bit application it takes advantage of more than 4GB of RAM. It utilizes all CPU cores with Grand
Central Dispatch. Open CL support allows GPU accelerated processing for improved performance for playback, rendering, and transcoding. It is resolution-independent, supporting images sizes from SD to beyond 4K. Final Cut Pro X supports
playback of many native camera and audio formats. It can also transcode video clips to the Apple ProRes codec for improved performance. Many tasks are performed in the background such as auto-saving, rendering, transcoding, and media
management, allowing the user an uninterrupted experience. Final Cut Pro X was developed for macOS only.

#### Workflow integration

##### Motion 5

Titles, motion graphics, effects generated in Motion 5 can be published to Final Cut Pro X. Inside the Final Cut Pro X, editors can modify the parameters and contents of the effects, as long as the permission for such modifications is
turned on in the Motion 5 project file.

##### Adobe Photoshop

In Final Cut Pro X 10.0.3 and later, the editor can import Photoshop projects onto the storyline similar to a still image. A Photoshop project with layers is treated similar to a compound clip and the layers are preserved after being
imported into the Final Cut Pro X. Individual layers of the Photoshop project can be toggled on or off inside the Final Cut Pro X by double-clicking the imported project and going into the compound clip editing panel. Other adjustments
to the Photoshop project should be performed on the imported Photoshop project using Adobe Photoshop program with updates happening in real-time inside Final Cut Pro X.

### Ecosystem

Before version 10, Final Cut Pro could be extended using the FXScript scripting language.

Since its release, Final Cut Pro X has supported the construction of effect, transition, and title plugins by publishing custom-built effects from Apple Motion. This has led to a third-party ecosystem of developers building effects from
simple color corrections to complex templates. Third-party plug-ins can also be created through Apple's FxPlug API, the successor of FXScript. As Projects, Events, and Libraries are stored in a database format; this has allowed many
third-party developers to build workflow tools by utilizing FCPXML.

### History

#### Creation

Randy Ubillos led the team that developed the first three versions of Adobe Premiere. His group was then hired by Macromedia to develop KeyGrip, a more professional video editing program based on Apple's QuickTime, for Macromedia. Niya
C Sisk was retained by Macromedia to create the UI of KeyGrip in partnership with the engineering team. However, Macromedia was unable to release the product, since they had licensed a component from Truevision, and the latter had a
licensing agreement with Microsoft that prohibited the component's use in conjunction with QuickTime. As a result, and due to Macromedia's decision to focus on the web market, it sold its desktop applications, including KeyGrip.

In 1998, KeyGrip was renamed Final Cut, and was demonstrated as a 0.9 alpha in a private room at the NAB Show. The
demonstration showed both Mac and Windows versions of the
software, with the Mac version using a Truevision RTX dual-stream real-time card with limited real-time effects. When no
buyer was found for the program, Apple acquired the
development team as a defensive measure. As Apple was unable to find a buyer for Final Cut, it continued development
work, adding FireWire support and releasing the program as
Final Cut Pro at NAB 1999.

#### Early versions

To ensure that Final Cut Pro had strong support for third-party self-paced and instructor-led training from the start, Apple partnered with DVcreators.net to release a training disc called "Final Cut Pro PowerStart" at the NAB show on
the day of Final Cut Pro's release. Apple also worked with DVcreators.net to host hundreds of free and paid Final Cut Pro seminars and workshops in 60 cities around the world in the following years, a strategy that some credit with
significantly contributing to Final Cut Pro's early market awareness and success.

After the release of Final Cut Pro, Adobe Premiere maintained a strong market share on Windows, but began to decline on Mac as its older codebase was more difficult to maintain. In 2003, Apple launched a trade-in program that allowed
Premiere users to exchange their discs for a free copy of Final Cut Express or receive a $500 discount on Final Cut Pro.

One of the factors that contributed to the success of Final Cut Pro was the relative maturity of QuickTime and its native support for new DV cameras connected via FireWire. The first fully broadcast quality, globally distributed TV show
produced using Final Cut Pro was Women of Wrestling in 2000, which used the Pinnacle CinéWave uncompressed video card. The Oxygen Network also used the software to produce shows such as SheCommerce during its network launch in early 2000.

In late 2001, independent producer Michael A. Bloom credited Final Cut Pro as being crucial to the production of his controversial film PlayCouples, A New Era of Swinging (2003). In an interview with Larry King, Bloom claimed that the
relatively new platform did not fail once while rendering the film, unlike his experiences with Avid Media Composer. Bloom had been an advocate for Final Cut Pro since using it for beta testing under an agreement between his production
company and The Oxygen Network. The studio motion picture The Rules of Attraction was also edited using beta versions of Final Cut Pro 3, demonstrating that successful 3:2 pulldown matchback to 24fps was possible with an easy-to-use
software product. The film's director, Roger Avary, became a spokesperson for Final Cut Pro, appearing in print advertisements worldwide. His endorsement of the product helped to give mainstream editors like Walter Murch confidence in
its readiness for professional use. In August 2002, Final Cut Pro received a Primetime Emmy Engineering Award for its impact on the television industry.

#### Final Cut Pro 4 to 7

Final Cut Pro 4 was released in April 2003, and included three new applications: Compressor for transcoding between video formats, LiveType for advanced titling (such as the creation of animated lower thirds), and Soundtrack for
creating royalty-free music soundtracks. It also included Cinema Tools, which had previously been sold separately for filmmakers working with telecine.

In April 2004, Final Cut Pro 4.5 was released and branded as "Final Cut Pro HD" due to its native support for Panasonic's tape-based DVCPRO HD format for compressed 720p and 1080i HD over FireWire. (While the software had been capable
of uncompressed HD editing since version 3.0, it required expensive video cards and high-speed storage at the time.)

Final Cut Pro 5 was announced at a pre-NAB event in April 2005 and shipped in May of that year. It added support for the HDV format for compressed HD, which had previously been supported in Final Cut Pro's scaled-down cousin, Final Cut
Express. Final Cut Pro 5 also added support for Panasonic's P2 format, which allowed for the recording of DVCPRO HD video to memory cards rather than tape.

In January 2006, Apple stopped selling Final Cut Pro as a standalone product and began offering it only as part of the Final Cut Studio bundle. In March 2006, a universal binary 5.1 version of Final Cut Pro was released as part of Final
Cut Studio, and upgrades were made available by sending the original installation discs back to Apple with a fee. One notable difference in the Intel versions of Final Cut and Motion was that they no longer recognized After Effects
plugins, but instead supported Apple's own universal plugin architecture, FxPlug.

On April 15, 2007, Apple unveiled Final Cut Pro 6 as the centerpiece of the Final Cut Studio 2 bundle. Despite not having a booth at NAB 2009, the product was widely represented on the show floor by various vendors, including the Red
Digital Cinema team, which relied heavily on Final Cut Pro during development.

On July 23, 2009, Final Cut Pro 7 (also referred to informally by users as Final Cut Studio 3) was released, though it remained a 32-bit application.

#### Final Cut Pro X

Final Cut Pro X was unveiled on April 12, 2011 at the NAB Show, and released to the Mac App Store on June 21, 2011 along with new versions of Motion and Compressor. Final Cut Pro X was fully-rewritten in 64-bit, with a new interface,
workflow enhancements and improved automation, and new features such as ColorSync integration, a resolution-independent playback system, and Core Animation-based system scaling. As part of the release, Final Cut Studio was discontinued,
along with Color, Soundtrack Pro, and DVD Studio Pro.

The reaction was extremely mixed, with veteran film editor Walter Murch initially refusing to use it, citing a lack of features compared to Final Cut Pro 7. Support for translating timelines from Final Cut Pro 7 to Final Cut Pro X was
notably missing, requiring editors to preserve a copy of Final Cut Pro 7 to edit older projects. An online petition asking Apple to continue development of Final Cut Pro 7 or to sell it to a third-party gathered 1,600 signatures within
a week. Some of the missing features in Final Cut Pro X that were essential for professional video production included the lack of an edit decision list (EDL), XML and Open Media Framework Interchange (OMF) support, the inability to
import projects created in previous versions of Final Cut Pro, the absence of a multicam editing tool, missing support for third-party I/O hardware output, and videotape capture being limited to FireWire video devices, including capture
with third-party hardware. These missing features were addressed within the first six months of the product's life. EDL export, a product of the early days of videotape editing, is now supported through third-party software and creating
an AAF (a newer version of OMF) for passing projects to Pro Tools through X2Pro. In a 2015 interview, Murch was much less critical of the tool and suggested that he was interested in using it.

One of the notable changes introduced in Final Cut Pro X was the Magnetic Timeline, which replaced the track-based timeline of previous versions. This initially caused issues with exporting audio stems for broadcast and distribution,
but this was addressed with the release of version 10.0.1, which introduced Video and Audio Roles, allowing users to export multitrack QuickTime files or stems. Files can be exported as AFF using a third-party app called X2Pro or
through Logic Pro X.

With version 10.0.6 released on October 23, 2012, Apple added native support for Redcode Raw and MXF through a third party plugin. Prior to the introduction of version 10.1, Project and Event Libraries were separate folders. Events
contained all the original media and Project Libraries contained the actual edited Projects on timelines. The Project and Event Libraries were stored in a user's Movie folder or on the root level of an external hard drive. These Libraries
automatically opened in Final Cut Pro X depending on which hard drives were mounted. That all changed on December 19, 2013, when Project and Event Libraries were merged into a new Library model. Libraries contained Events which in turn
contained Projects. And unlike before Libraries could be opened and closed by the user. Media could be stored internally in the Library or kept outside the Library. Media management was further refined in version 10.1.2, released on
June 27, 2014. MXF import, edit, and export became natively supported with version 10.1.4.

Version 10.2, released during the NAB Show 2015, introduced 3D Titles in both Final Cut Pro X and Motion. The Color Board was merged with a new Color Correction effect to allow for more flexibility in stacking layers of effects, and
Apple added the ability to apply Keying or Shape Masks to any effect. Version 10.3 introduced a redesigned interface with Magnetic Timeline 2, support for iXML metadata when importing audio, significantly improved audio editing, support for
wide-gamut color and REC 2020 color import, edit, and export, and support for MXF-wrapped Apple ProRes.

Version 10.4 introduced color wheels and color curves, 360º video editing, and high-dynamic-range (HDR) video, and the HEVC and HEIF formats. In April 2018, Apple said that there were more than 2.5 million users of Final Cut Pro X. In
version 10.4.1, released during the NAB Show 2018, closed captioning was added, along with support for ProRes RAW. In November 2020, in tandem with the release of macOS Big Sur, the X was dropped from the name, and the product became
again known as Final Cut Pro.

#### Final Cut Pro for iPad

Final Cut Pro for iPad was released on May 23, 2023. It requires an iPad with an M-series chip and is available only through the software as a service model for $4.99 a month or $49 a year.