# HGT GM MIDI Mapping v1.0

**Status:** Specification baseline 1.0  
**Owner:** HGT – Hans-Georg Tröster  
**Scope:** Genre Converter, Genre Remap, Drum Construction Kit  
**MIDI standard basis:** General MIDI Level 1 percussion key map  
**Canonical percussion channel:** MIDI channel 10 (fixed; not user-configurable)

## 1. Purpose

This document defines the shared MIDI percussion mapping used by all three HGT Ableton extensions. It is the single source of truth for instrument note numbers, the ten-instrument standard layout, genre-dependent visibility, velocity handling, and HGT global Control Change (CC) assignments.

The mapping is independent of any one extension's user interface or internal implementation. Extensions may expose different features, but they must not redefine the canonical note numbers or CC assignments.

## 2. Binding decisions

- GM percussion note range: **35–81 inclusive** (47 note numbers).
- Ten fixed standard instrument slots, shown in the same order in all three extensions.
- Step Sequencer instrument visibility is **genre-dependent**. Hiding an instrument must never change or renumber its MIDI note.
- Percussion notes and HGT CC messages use **MIDI channel 10** (MIDI channel number 10; zero-based status-channel index 9 in raw MIDI bytes).
- HGT CC architecture is **global**: CC 20–29 control extension-wide parameters, not individual drum instruments.
- Instrument identity is carried by MIDI Note Number, not by CC.
- Velocity is independent of CC and is carried by the Note On velocity value.
- Octave labels in HGT documentation use the convention **C1 = MIDI note 36**. MIDI note number is authoritative if another application displays a different octave name.

## 3. Ten-instrument standard layout

The following ten slots are fixed and must appear in this order when the standard layout is shown. The two-row arrangement is five instruments per row, matching the established HGT interface reference.

| Slot | HGT display name | GM instrument | MIDI note | HGT octave label |
|---:|---|---|---:|---|
| 1 | Kick | Bass Drum 1 | 36 | C1 |
| 2 | Snare | Acoustic Snare | 38 | D1 |
| 3 | Rim / Side Stick | Side Stick | 37 | C♯1 |
| 4 | High Tom | Hi-Mid Tom | 48 | C2 |
| 5 | Mid Tom | Low Tom | 45 | A1 |
| 6 | Floor Tom | Low Floor Tom | 41 | F1 |
| 7 | Closed Hi-Hat | Closed Hi-Hat | 42 | F♯1 |
| 8 | Open Hi-Hat | Open Hi-Hat | 46 | A♯1 |
| 9 | Crash | Crash Cymbal 1 | 49 | C♯2 |
| 10 | Ride | Ride Cymbal 1 | 51 | D♯2 |

The display names are concise HGT UI labels. The GM instrument names and note numbers define the standard mapping. In particular, the HGT labels “High Tom” and “Mid Tom” are aliases for GM notes 48 and 45 respectively; they must not be silently reassigned.

## 4. Complete GM Level 1 percussion map (35–81)

| MIDI note | HGT octave label | GM instrument name |
|---:|---|---|
| 35 | B0 | Acoustic Bass Drum |
| 36 | C1 | Bass Drum 1 |
| 37 | C♯1 | Side Stick |
| 38 | D1 | Acoustic Snare |
| 39 | D♯1 | Hand Clap |
| 40 | E1 | Electric Snare |
| 41 | F1 | Low Floor Tom |
| 42 | F♯1 | Closed Hi-Hat |
| 43 | G1 | High Floor Tom |
| 44 | G♯1 | Pedal Hi-Hat |
| 45 | A1 | Low Tom |
| 46 | A♯1 | Open Hi-Hat |
| 47 | B1 | Low-Mid Tom |
| 48 | C2 | Hi-Mid Tom |
| 49 | C♯2 | Crash Cymbal 1 |
| 50 | D2 | High Tom |
| 51 | D♯2 | Ride Cymbal 1 |
| 52 | E2 | Chinese Cymbal |
| 53 | F2 | Ride Bell |
| 54 | F♯2 | Tambourine |
| 55 | G2 | Splash Cymbal |
| 56 | G♯2 | Cowbell |
| 57 | A2 | Crash Cymbal 2 |
| 58 | A♯2 | Vibraslap |
| 59 | B2 | Ride Cymbal 2 |
| 60 | C3 | Hi Bongo |
| 61 | C♯3 | Low Bongo |
| 62 | D3 | Mute Hi Conga |
| 63 | D♯3 | Open Hi Conga |
| 64 | E3 | Low Conga |
| 65 | F3 | High Timbale |
| 66 | F♯3 | Low Timbale |
| 67 | G3 | High Agogo |
| 68 | G♯3 | Low Agogo |
| 69 | A3 | Cabasa |
| 70 | A♯3 | Maracas |
| 71 | B3 | Short Whistle |
| 72 | C4 | Long Whistle |
| 73 | C♯4 | Short Guiro |
| 74 | D4 | Long Guiro |
| 75 | D♯4 | Claves |
| 76 | E4 | Hi Wood Block |
| 77 | F4 | Low Wood Block |
| 78 | F♯4 | Mute Cuica |
| 79 | G4 | Open Cuica |
| 80 | G♯4 | Mute Triangle |
| 81 | A4 | Open Triangle |

## 5. Genre-dependent instrument visibility

The complete map is always available to the mapping engine. The Step Sequencer may show a genre-specific subset to keep the interface clear. Visibility is a presentation rule only; it does not alter MIDI note numbers, remove support from imported files, or rewrite existing MIDI clips.

Suggested initial visibility profiles:

| Genre profile | Additional suggested GM notes | Instruments |
|---|---|---|
| Classic Rock | 40, 44, 54, 57 | Electric Snare, Pedal Hi-Hat, Tambourine, Crash 2 |
| Blues Rock | 44, 51, 53, 54 | Pedal Hi-Hat, Ride 1, Ride Bell, Tambourine |
| Alternative Rock | 40, 50, 52, 55, 57 | Electric Snare, High Tom, Chinese Cymbal, Splash, Crash 2 |
| Punk | 40, 43, 47, 50, 55, 57 | Electric Snare, High Floor Tom, Low-Mid Tom, High Tom, Splash, Crash 2 |
| Funk | 39, 40, 44, 54, 56, 60–64, 69–70 | Clap, Electric Snare, Pedal Hi-Hat, Tambourine, Cowbell, Congas/Bongos, Cabasa, Maracas |
| Reggae | 37, 39, 44, 54, 56, 60–64, 69–70 | Side Stick, Clap, Pedal Hi-Hat, Tambourine, Cowbell, Congas/Bongos, Cabasa, Maracas |
| Ska | 39, 44, 54, 56, 65–70 | Clap, Pedal Hi-Hat, Tambourine, Cowbell, Timbales, Agogo, Cabasa, Maracas |
| Hip-Hop | 35, 39, 40, 54, 56, 69–70 | Acoustic Bass Drum, Clap, Electric Snare, Tambourine, Cowbell, Cabasa, Maracas |

These are initial display suggestions, not restrictions on what a user may play. A user-created or imported pattern may contain any supported GM note from 35–81.

## 6. MIDI channel and event rules

### 6.1 Channel

- Use MIDI channel 10 for all GM percussion Note On, Note Off, and HGT CC 20–29 messages.
- Channel 10 is fixed and must not be exposed as a user-selectable setting in the HGT GM MIDI Mapping v1.0 implementation.
- In raw MIDI status bytes, channel 10 is represented by channel index 9 (for example, Note On status `0x99`, Control Change status `0xB9`).

### 6.2 Notes and velocity

- Valid GM percussion note numbers in this specification: 35–81.
- Valid Note On velocity: 1–127.
- A Note On with velocity 0 is interpreted as Note Off, as required by MIDI convention.
- Velocity layers, accents, ghost notes, and humanization may change velocity but must not change the instrument's note number.
- Note duration and Note Off handling remain the responsibility of the MIDI event generator/player.

### 6.3 Hi-hat articulation and choke

- Closed Hi-Hat: note 42.
- Pedal Hi-Hat: note 44.
- Open Hi-Hat: note 46.
- Where the target drum instrument supports choke groups, notes 42 and 44 should choke/terminate a currently sounding open hi-hat note 46. The MIDI mapping itself does not guarantee that every third-party sound library implements this behavior; the Drum Rack/device configuration must provide it.

## 7. HGT global CC mapping

All CC assignments below are global extension controls. They are not per-pad or per-instrument controls. All messages use MIDI channel 10. The CC numbers 20–29 are an HGT-defined private convention for this workflow; they are not GM instrument selectors and must be documented as HGT-specific assignments.

| CC | Parameter | Value interpretation |
|---:|---|---|
| 20 | Performance Feel | 0–127 normalized control; extension maps to its Performance Feel range |
| 21 | Swing | 0–127 normalized control; 0 = minimum/no added swing, 127 = maximum configured swing |
| 22 | Fill Intensity | 0–127 normalized control; 0 = minimum, 127 = maximum configured fill intensity |
| 23 | Groove Variation | 0–127 normalized control; 0 = minimum, 127 = maximum configured variation |
| 24 | Verse Variation | 0–127 normalized control for the selected verse-variation behavior |
| 25 | Song Dramaturgy | 0–127 normalized control for the extension's dramaturgy/tension setting |
| 26 | Repetition / Pass | Discrete selector: 0 = First Pass, 1 = Second Pass, 2 = Final Pass, 3 = Repeat/Loop; 4–127 reserved |
| 27 | Drummer Style Influence | 0–127 normalized control; 0 = minimum influence, 127 = maximum influence |
| 28 | Preview Volume | 0–127 normalized preview output level |
| 29 | Master Variation | 0–127 normalized global variation control |

### 7.1 CC implementation requirements

- Each CC number has one global meaning across all HGT extensions.
- Do not reuse one of these CC numbers for a different parameter in another extension.
- Do not assign these CCs to individual drum pads.
- CC values are 7-bit unsigned integers (0–127).
- For continuous parameters, map 0–127 linearly or through a documented parameter curve to the receiving parameter's native range.
- CC 26 uses the fixed enum: 0 = First Pass, 1 = Second Pass, 2 = Final Pass, 3 = Repeat/Loop. Values 4–127 are reserved and must be ignored. Do not infer other meanings from intermediate values.
- A receiving extension may ignore a CC for a feature it does not implement, but it must not reinterpret that CC as another parameter.
- CC 28 (Preview Volume) affects preview monitoring only; it must not change the velocity or dynamics of exported/generated MIDI notes.
- CC 20–29 are HGT workflow controls. They are not stored as drum hits and must not be confused with the GM percussion note map.

## 8. Extension conformance

Each extension conforms to this specification when it:

1. Uses the fixed ten-instrument layout and exact note numbers in Section 3.
2. Recognizes the complete GM percussion range 35–81 for import/export or mapping wherever the extension handles percussion notes.
3. Keeps genre-dependent visibility separate from MIDI note identity.
4. Uses MIDI channel 10 for generated GM percussion and HGT CC messages.
5. Implements the shared CC meanings without local reassignment.
6. Preserves unknown or currently hidden GM percussion notes when processing a MIDI file, unless the user explicitly requests their removal or remapping.
7. Does not silently transpose, renumber, or octave-shift notes to compensate for another application's octave-label convention.

## 9. Compatibility and implementation notes

- MIDI note numbers are authoritative; octave labels are display metadata only.
- Third-party drum instruments may use non-GM mappings. Any translation to EZdrummer, Battery, Kontakt, Drumlogue, or another custom map must be an explicit mapping profile layered on top of this canonical HGT GM map. It must not modify the canonical GM definitions.
- Live 13 integration, Drum Rack construction, Push layouts, and Step Sequencer behavior are implementation projects that consume this specification; they are not guaranteed merely by defining the mapping.
- The JSON file `HGT_GM_MIDI_MAPPING_v1.0.json` is the machine-readable companion and must remain semantically consistent with this document.

## 10. Change control

Changes to canonical note numbers, the ten standard slots, channel 10, or CC meanings require a new specification version and coordinated updates to all three extensions. Genre visibility profiles may be extended without changing the core mapping version, provided they do not alter note identity or CC semantics.
