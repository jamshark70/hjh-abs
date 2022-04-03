## hjh-abs

A small collection of only loosely maintained Pure Data utility abstractions.

- dataseq-hjh.pd: One-row-at-a-time sequencer.
- eg-hjh~.pd: ADSR.
- fader~ suite: Modular mixing abstractions with wireless connections and support for send aux effects.
- lfo-norm-hjh~.pd: Multimode LFO.
- midimonoglide and noteglide: Preprocessing incoming MIDI messages to mimic "legato"-style monosynths.
- moving-avg.pd: Smoothing filter.
- moving-median.pd: Smoothing filter (depends on cyclone).
- pm-hjh~.pd: Phase modulation oscillator.
- rand3.hjh.pd: Triplet of random numbers.
- seq-hjh.pd: Timed sequencer.
- sf-scale-ms.pd: Adapt ms for file sample rate.
- sf-startmsgd.pd: "Start" message for [play~].
- sf-startmsg.pd: "Start" message for [play~].
- soundfiler2.pd: Soundfiler with more stats.
- [stereofile] and [monofile] audio file managers. Essentially a wrapper for [soundfiler2] that manages array(s) for you, and interfaces with audio file players.
- [sf-play~], [sf-play2~], [sf-varispeed~], [sf-varispeed2~]: Audio file players that connect to arrays managed by [stereofile] and [monofile], with crossfade looping support.
- tick-scheduler: A message scheduler based on incoming ticks, suitable for use with clock sources such as [metro], [abl_link~] or MIDI clock messages.
- vstplug-hjh~.pd: Wrapper for vstplugin~.

### Dependencies

- Dependencies available from deken.
  - Cyclone.
  - [recorder~] depends on zexy.
  - [tick-scheduler] depends on pdcontainer.
  - [fader~] and related objects depend on iemguts.
  - [formlet~] depends on the ELSE library.
  - Many help patches use pddp/ezoutput~.
- Other dependencies:
  - [vstplug-hjh~] depends on Christof Ressi's excellent vstplugin~ external, available at https://git.iem.at/pd/vstplugin .

### Acknowledgements

Many of these abstractions would not exist without valuable advice from the Pure Data user forum at https://forum.pdpatchrepo.info/, and from developer discussions in the Pd issue tracker at https://github.com/pure-data/pure-data.

Specific credit is due to the following:

- Pd forum user lacuna posted [a formula for `[in-range~]`](https://forum.pdpatchrepo.info/topic/13644/inrange-in-vanilla-any-improvements/3) that is far better than my own, which I have used.
- The [fader~] family depends on "dynamic catch~" objects authored by Christof Ressi.
