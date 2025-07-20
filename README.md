# Frostmod Audio: Riffline

Welcome to Frostmod Audio's first plugin - the Drumlogue plugin Riffline.

In an attempt to be the change one wants to see, namely a better ecosystem for an underappreciated drum/plugin machine, I decided to start creating some of the plugins I myself would use on it.

## What is it?

Riffline is a dual voice (for now) single oscillator supersaw type synthesizer plugin with a few modulation options and a switchable HP/LP filter.

## Release status

Public beta

## Availability

Riffline is available for free, currently in the releases section of this repository while I work on a Frostmod Audio website. The intention is to keep this plugin as a free/donation plugin.

## Known issues/limitations/what are we working on?

- It's still a little CPU hungry which has made it difficult to add more voices. I'm trying to improve on the voicing structure so I can add more voices to it and lower the CPU usage.
- Voice stealing currently works by rotating the voices, which can lead to unexpectedly cut notes if using it polyphonically with a MIDI keyboard/sequencer.
- Note switching will introduce crackles when played reasonably fast with external MIDI keyboard/sequencer.

## Interface

Still working on proper documentation which will be part of the 1.0 release. Controls are listed underneath each page below, with short descriptions numbered left to right 1-4:

### Page 1

Oscillator settings

1. PITCH - Sets the note triggered by the Drumlogue sequencer. Does not affect MIDI sequencing
2. ENV PTCH - Pitch modulation amount for envelope 2
3. DETUNE - Detune spreads the 7 saw oscillators creating a supersaw effect
4. BLEND - Sets the level of the 6 additional saws of the 7 saw oscillator in relation to the main saw oscillator

### Page 2

Filter settings

1. FLT TYPE - Switch between the HP2 and LP2 filter types
2. FILTER - Controls the filter frequency
3. RES - Controls the filter resonance
4. ENV FLT - Sets the amount of modulation applied to the filter frequency from envelope 2

### Page 3

LFO Settings

1. LFO SPD - Controls the rate of the LFO
2. ENV SPD - Sets the amount of modulation on LFO rate from envelope 2
3. LFO PTCH - Sets the amount of modulation on Pitch from the LFO
4. LFO FLT - Sets the amount of modulation on filter frequency from the LFO

### Page 4

Controls the AMP envelope which is an AHR envelope, Attack, Hold, and Release

1. ATTACK - Attack of AMP envelope
2. RESERVED
3. RELEASE - Release of the AMP envelope
4. RESERVED

### Page 5

Envelope 2 settings. Envelope 2 is a ADHR envelope which will hold if Decay is not set

1. ENV ATK - Attack of envelope 2
2. ENV DEC - Decay of envelope 2, if set to 0 the envelope will hold until released.
3. ENV REL - Release of envelope 2
4. RESERVED

### Page 6

1. OSC VOL - Controls the volume of the oscillator. Usefull when high resonance causes unwanted clipping
2. RESERVED
3. RESERVED
4. RESERVED