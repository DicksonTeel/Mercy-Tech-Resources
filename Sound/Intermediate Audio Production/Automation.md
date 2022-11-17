# Automation
*Automation: Events referencing time*

## Events

- Fader moves
- Cuts/Mutes
- Pan
- Aux level/mute/pan
- EQ/Dynamics
- Virtually any parameter


 ## Time
- SMPTE
- MTC
- DAW timeline


## Real-time Automation Modes

- Write/Absolute: Used to record new automation data or to record over existing data.
- Read/Replay: Used to playback existing automation data. Nothing new is recorded.
- Trim/Relative: Used to edit existing automation data.
- Off/Manual: Automation is disabled.
 
- These modes can be global or on a per channel basis.


### Additional Automation Modes
- **Determine how to get into writing automation & how to get out of writing automation.**

- Touch/return/snap: Automation data is only being written while the fader is being “touched”, afterward it switches back to Read.
- Latch: Automation data is written when the fader is touched, but the parameters stay in record when the fader is released.
- Automatch: Fader returns (or other control) returns to the previous automated position when exiting a record Mode.
- To End: The current position of a control is written to the end of a mix when exiting a record Mode.
- To Next/Previous/Punch: The current position of a control is written to next or previous data when exiting a record Mode.

- These modes can be global or on a per channel basis.

---
## Automation Workflow
- **Get a relative blend and basic sounds before starting automation. Compressor & EQ settings can affect levels and therefore should be decided upon before automation.**

- Automation uses breakpoints that are arranged on a line. Automation is contained in an Automation “playlist”, one for each parameter. The good thing about breakpoints is that they allow for graphical entry and editing. Before automation begins there is an “initial” breakpoint (this is where the parameters are to begin with). Automation for tracks is “always on” (unless specifically suspended) but plugin parameters need to be “auto enabled” individually, but the basic volume, pan, and mute are always enabled. Automation types can be enabled/disabled globally. You can also add “lanes” to view multiple - editable - automation parameters at the same time.

---
## Freeze and Commit
### Freeze

- Offline renders a track to free up processing power and reduce latency.
- Used as a Temp solution.
- Can be done to the entire track or up to a select insert.
- Cannot make any more adjustments to the processing on a frozen track until it is unfrozen.
- Control is maintained over: Volume/Mute/Pan/Send Level/Send Mute/Send Pan/Plugin automation for plugins that are not frozen.
- Control is lost over: Edit clips/changing elastic audio/render audio suite plugins/ change temp or song start, or enable or disable Conductor track/insert or cut time.

### Commit

- Creates a copy of a track with its processing.
- Is used to future proof a track, free up CPU on completed tracks, or send to other users.
- Can commit the whole track or just the edit section.