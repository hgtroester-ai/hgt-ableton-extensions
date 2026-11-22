# HGT GM Instrument Layout v1.0

This is the UI-facing companion to `HGT_GM_MIDI_MAPPING_v1.0.md`.

## Standard layout

Show five instruments per row, in this exact order:

| Row | Position | Display name | MIDI note |
|---:|---:|---|---:|
| 1 | 1 | Kick | 36 |
| 1 | 2 | Snare | 38 |
| 1 | 3 | Rim / Side Stick | 37 |
| 1 | 4 | High Tom | 48 |
| 1 | 5 | Mid Tom | 45 |
| 2 | 1 | Floor Tom | 41 |
| 2 | 2 | Closed Hi-Hat | 42 |
| 2 | 3 | Open Hi-Hat | 46 |
| 2 | 4 | Crash | 49 |
| 2 | 5 | Ride | 51 |

Each item displays its HGT name and MIDI note label/number. The MIDI note number is the authoritative value. Use the octave labels from the core mapping only as display labels.

## Genre-dependent rows

The ten standard slots remain the stable core. Genre-specific GM instruments outside the ten slots may be shown in an additional/expanded area when relevant to the selected genre. Hiding an instrument is not permission to discard its MIDI events.

## UI compatibility

The established HGT two-row, five-column arrangement is the reference layout. Do not redesign the existing extension interface as part of adopting the mapping. The shared mapping is a data and behavior standard, not a mandate to make all extension windows identical in every other respect.
